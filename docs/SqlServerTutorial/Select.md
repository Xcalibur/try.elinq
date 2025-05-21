# SQL Server SELECT

- [A) `SELECT` – retrieve some columns of a table](#a-sql-server-select--retrieve-some-columns-of-a-table)
- [B) `SELECT` – retrieve all columns from a table](#b-sql-server-select--retrieve-all-columns-from-a-table)
- [C) `SELECT` – sort the result set](#c-sql-server-select--sort-the-result-set)
- [D) `SELECT` – group rows into groups example](#d-sql-server-select--group-rows-into-groups-example)
- [E) `SELECT` – filter groups example](#e-sql-server-select--filter-groups-example)

ELINQ extends `DbSet` with a `Query` method. As any LINQ method, it accepts a Lambda. The Lambda parameters are the entities we want to participate in the query and return value is the result of `SELECT` invocation:

### A) SQL Server `SELECT` – retrieve some columns of a table

Retrieving some columns is not a common case in EF and requires declaration of the dedicated keyless entity (`FullName`).

```cs --project ../../../SqlServerTutorial/SqlServerTutorial.csproj --source-file ../../../SqlServerTutorial/Basic/Select.cs --region A
```

Another option is to use LINQ for the anonymous top level projection. See how easy is to mix ELINQ and LINQ:

```cs --project ../../../SqlServerTutorial/SqlServerTutorial.csproj --source-file ../../../SqlServerTutorial/Basic/Select.cs --region A_1
```

### B) SQL Server `SELECT` – retrieve all columns from a table

```cs --project ../../../SqlServerTutorial/SqlServerTutorial.csproj --source-file ../../../SqlServerTutorial/Basic/Select.cs --region B
```

### C) SQL Server `SELECT` – sort the result set

```cs --project ../../../SqlServerTutorial/SqlServerTutorial.csproj --source-file ../../../SqlServerTutorial/Basic/Select.cs --region C
```

### D) SQL Server `SELECT` – group rows into groups example

```cs --project ../../../SqlServerTutorial/SqlServerTutorial.csproj --source-file ../../../SqlServerTutorial/Basic/Select.cs --region D
```

### E) SQL Server `SELECT` – filter groups example

```cs --project ../../../SqlServerTutorial/SqlServerTutorial.csproj --source-file ../../../SqlServerTutorial/Basic/Select.cs --region E
```

---

[< BACK](Basic.md) | [HOME](/)
