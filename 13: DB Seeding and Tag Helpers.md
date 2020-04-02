# Reading 13: DB Seeding and Tag Helpers

## Microsoft Docs: Data Seeding
- The process of populating a database with an initial set of data
- Several ways this can be accomplished in EF Core:
  - Model seed data
    - Seeding data can be associated with an entity type as part of the model configuration.
    - Then, the migrations can automatically compute what insert, update, or delete operations
    - Limitations: primary key needs to be specified, previously seeded data will be removed if the primary key is changed in any way
      - Therefore, most useful for static data that's not expected to change outside of migrations and does not depend on anything else in the database (Ex: zip codes)
  - Manual migration customization
    - Manual addition of InsertData(), UpdateData(), or DeleteData()
  - Custom initialization logic
    - DbContext.SaveChanges()
