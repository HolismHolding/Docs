# Controller

Read-only controllers should inherit from `ReadController<ReadModel>`

Read-write controllers should inherit from `Controller<ReadModel, WriteModel>`

Read-only tree structures should inherit from `ReadTreeController<ReadModel>`

Read-write tree structures should inherit from `TreeController<ReadModel, WriteModel>`

If there is no model related to the controller, inherit it from `HolismController`

If you need to access all data on the client, it is a `ClientLookup` controller. It should inherit from `ClientLookupReadController<ReadModel>` or `ClientLookupController<ReadModel, WriteModel>` based on read-write requirements.

Site controllers that are related to an entire module, should be named `ModuleNameController` and should expose a `Data` action.

Site controllers that are related to a main entity inside a module, should expose an action named `Get`.
