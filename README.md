ACL Builder Utilility for Elgg
==============================

## Features

 * API for creating an access collection for a set of users

## Notes

 * This plugins allows you to create access collections on the fly, if you need
to limit access to a certain entity to a set of predefined users. Created access
collections are permnanent, and the access collection IDs will always refer to the same
set of users, and thus can be recycled.

## Usage

```php
use hypeJunction\Access\Collection;
$entity->access_id = Collection::create(array($user1, $user2))->getCollectionId();
```
