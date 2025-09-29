## SQL Police Department - Solutions

SQL Police Department is an educational web site for learning or improving SQL through practical exercises in the form of “investigative cases.”

These are the solution for all free cases. Furthermore, it is required to buy a license to continue to solve cases.

I noticed that restarting the game several times changes the context and variables for solving cases, but the structure of the queries remains the same.

###### Case #1

A hacked site subscribers' details have surfaced on a darknet forum. Please submit all subscribers' details.

```SQL
SELECT *
FROM subscribers;
```

###### Case #2

A mailing list of an illegal online service was sent to the SQLPD hot-line. Please submit all records' details.

```SQL
SELECT *
FROM records;
```

###### Case #3

An illegal site's servers were seized in a recent operation. Please submit all users given names and family names' details.

```SQL
SELECT GivenName, FamilyName
FROM users;
```

###### Case #4

A mailing list of an illegal online service was sent to the SQLPD hot-line. Please submit all records given names, last names and number of promotions sent' details.

```SQL
SELECT GivenName, LastName, PromotionSent
FROM mailing_list;
```

###### Case #5

A hacked site members' details have surfaced on a darknet forum. Please submit all members number of purchases' details. Please make sure there are no duplicates.

```SQL
SELECT DISTINCT NumberOfPurchases
FROM members;
```

###### Case #6

An illegal site's servers were seized in a recent operation. Please submit all users' details sorted by number of posts in ascending order.

```SQL
SELECT *
FROM users
ORDER BY Posts ASC;
```

###### Case #7

A mailing list of an illegal online service was sent to the SQLPD hot-line. Please submit all records' details sorted by number of promotions sent in descending order.

```SQL
SELECT *
FROM mailing_list
ORDER BY Promotions DESC;
```

###### Case #8

A mailing list of an illegal online service was sent to the SQLPD hot-line. Please submit all records first names and emails' details sorted by emails in descending order. Please make sure there are no duplicates.

```SQL
SELECT DISTINCT FirstName, Email
FROM mailing_list
ORDER BY Email DESC;
```

###### Case #9

An illegal site's servers were seized in a recent operation. Please submit all users number of downloads, emails and last names' details sorted by number of downloads in ascending order and then by emails in ascending order.

```SQL
SELECT LastName, Email, Downloads
FROM users
ORDER BY Downloads ASC, Email ASC;
```

###### Case #10

An illegal site's servers were seized in a recent operation. Please submit the top 5 users' details when sorted by number of posts in ascending order and then by surnames in descending order.

```SQL
SELECT *
FROM users
ORDER BY NumberOfPosts ASC, Surname DESC
LIMIT 5;
```

###### Case #11

A mailing list of an illegal online service was sent to the SQLPD hot-line. Please submit the top 3 records join dates, number of password changes and surnames' details when sorted by join dates in ascending order and then by surnames in descending order. Please make sure there are no duplicates.

```SQL
SELECT DISTINCT Surname, JoinDate, PasswordChanges
FROM mailing_list
ORDER BY JoinDate ASC, Surname DESC
LIMIT 3;
```
