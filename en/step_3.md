TODO: Scrap the people. Create a timeline of periods only (or, at least, things that can be plotted directly).

## Discovering the people

Each era in time is defined by its people. You are now going to find a list of people who lived in your chosen historical period.

Recall that `HistoricalPeriodData[]` is a list of historical period entities. These entities contain information about periods in the past--in particular, they contain lists of notable figures who lived during them.

--- task ---

Find the properties of `HistoricalPeriodData[]`.

--- hints ---

--- hint ---

As `HistoricalPeriodData[]` is a list, you will need to use `EntityValue`.

--- /hint ---

--- hint ---

The code you need is:

```
EntityValue[HistoricalPeriodData[], "Properties"]
```

--- /hint ---

--- /hints ---

Using the appropriate property option (in its canonical form), find a list of notable historical figures.

--- hints ---

--- hint ---

The option you need is "PeopleInvolved".

--- /hint ---

--- hint ---

The code you need is:

```
EntityValue[HistoricalPeriodData[], "PeopleInvolved"]
```

--- /hint ---

--- /hints ---

--- /task ---

If you look at your list, you'll notice that it's quite a mess! There are several periods with no notable people (shown as "Missing[NotAvailable]") and others in which the people have no known properties (shown as plain text).

From this list, you would like to select those people who lived during your chosen period. To do so, you can use the function `Select`. This function takes all the items from a list that meet some criteria.

If an item doesn't meet the criteria precisely, then it will be ignored. Luckily for you, this means you don't have to worry about the missing or plain text data, as your criteria will concern entities.


First, let's find all of the people born before the end of your period.

--- task ---

Select

--- /task ---

