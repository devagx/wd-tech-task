# WD

The tar archive contains a snippet of legacy code inherited from another company.

For brevity, the implementation of the DatabaseSystem class is not included and can be assumed to function correctly.

The purpose of the code is:

-To receive an incoming Customer data record
-Validate the incoming record
-If the account has been active in the previous 5 days (inclusive) create or update a LocalCustomer record in a local data store
-If the account has not been active in the previous 5 days (inclusive) delete the LocalCustomer data from the data store (if it exists).

The goal of this exercise is to add a new feature to the code:
-Only delete records for personal accounts (not business accounts).
-This should be verified by a unit test.
-It is not required to implement the data layer.

Unfortunately, the inherited code is in a bad state and has various issues (misplaced validation, business logic not well separated from the data layer, dubious exception implementation among others) so refactoring is encouraged and all classes can be modified as you wish (though modifications to the DatabaseSystem and DataFactory are out of scope).

