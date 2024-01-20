# Business

If it's read only, inherit from `ReadBusiness<ReadModel>`

If it's read and write, inherit from `Business<ReadModel, WriteModel>`

If it's a recursive data structure, inherit from `Tree<ReadModel, WriteModel>`

Enums would inherit from `EnumBusiness<EnumType>`

And CLOB businesses would inherit from `ClobBusiness<ReadModel, WriteModel>`
