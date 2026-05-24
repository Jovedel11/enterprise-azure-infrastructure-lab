# Enterprise Azure Infrastructure Lab - Storage Phase

## Objective

- Create Blog Storag and Azure files, and explore what is the use for them.

## Storage Architecture

Storage Account
- Standard Storage.
- Hot Tier (For requently access).
- Blog Stroage for (Primary Service).
- LRS to mimimize cost.

## Design Decisions

- Create Container for Blob and add a file on it (Private if Public It can access by URL)
- Create File Share.
- Connect it in my Linux.
- After I open my Linux, I paste the Transcript provided.
- Access my File Share.

## Expected Learnings

- Where to create a container for Blob and upload a data to it.
- How to mouting cloud storage, attaching shared files.
- Access Shared Files using Linux.
- Demonstrate the architectural difference between object storage and share file system.
