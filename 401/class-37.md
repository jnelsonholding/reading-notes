### Class 37 Reading Notes

## Amazon S3

S3 is a data storage service that is flexible to your usage. It's web-accessed, cloud storage with service options that allow for varying use cases.

S3's data containers are called buckets. For a user, a bucket acts like a content directory that can be used like a database. They can be located regionally to provide quick access where they are needed as well.

The data stored in buckets is held as objects. Objects are uniquely identifiable through a combination of their bucket, their key (like a path within the bucket), and their version ID.

S3 is made to handle duplicate data held in different regions. This allows for quick access to the same data in very disparate locations. But in order to maintain this, S3 needs to handle writes and deletes carefully. In order to maintain consistency, S3 requires that a client first get fresh data and soon after handle their put or delete. This can result in a temporary stall in other requests for same data while normalizing across regions.

[Return to table of contents](../README.md)
