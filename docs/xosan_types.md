# XOSAN types

There is 2 modes for creating an XOSAN storage. They are different and the choice is done forever. You can't **switch from a mode to another** when XOSAN is created, except by removing and re-creating it.

That's why it's **very important to understand pros and cons** of each type.

> On "top" of there 2 types, you can also decide to spread all operations to multiple number of volumes. This is called **distributed** mode. It's very similar to *RAID 0*, which can be placed on top of a *RAID 1* for example. We'll talk about it in the end of this guide.

Here is those 2 types:

* [Replicated](xosan_replicated.md)
* [Disperse](xosan_disperse.md)

## Which mode to choose

In the vast majority of cases, **replicated is better**, because:

* it's almost ALWAYS faster
* it's easier to manage
* it's easier to grow

The only downside is that replicated will "waste" more space.

Using disperse makes sense only if:

* you have big HDDs and you want use the space at most
* you don't use database (or don't care about performances)
* you store big files and you don't need ultra fast data access