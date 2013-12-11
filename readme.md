<h1>Api rest with nodejs and mysql using forms</h1>

<p>Create a new table in your database for stored, update, delete and show users</p>
```mysql
--
-- Estructura de tabla para la tabla `users`
--
 
CREATE TABLE IF NOT EXISTS `users` (
  `id` int(10) unsigned NOT NULL AUTO_INCREMENT,
  `username` varchar(50) COLLATE utf8_unicode_ci NOT NULL,
  `email` varchar(100) COLLATE utf8_unicode_ci NOT NULL,
  `password` varchar(200) COLLATE utf8_unicode_ci NOT NULL,
  `created_at` timestamp NOT NULL DEFAULT '0000-00-00 00:00:00',
  `updated_at` timestamp NOT NULL DEFAULT '0000-00-00 00:00:00',
  PRIMARY KEY (`id`),
  UNIQUE KEY `users_email_unique` (`email`)
) ENGINE=InnoDB DEFAULT CHARSET=utf8 COLLATE=utf8_unicode_ci AUTO_INCREMENT=1 ;
 
/*!40101 SET CHARACTER_SET_CLIENT=@OLD_CHARACTER_SET_CLIENT */;
/*!40101 SET CHARACTER_SET_RESULTS=@OLD_CHARACTER_SET_RESULTS */;
/*!40101 SET COLLATION_CONNECTION=@OLD_COLLATION_CONNECTION */;
```

## Url for add new users

http://localhost:3000/create

## Url for update users, where 1 is userid

http://localhost:3000/user/update/1

## Url for delete a user by id

http://localhost:3000/delete

## Url for show all users in json format

http://localhost:3000/users

## Url for show one user in json format by userid

http://localhost:3000/users/1



## Tutorial in spanish language

* [Tutorial](http://uno-de-piera.com/api-rest-con-node-js-express-y-mysql/)

## Visit me

* [Visit me](http://uno-de-piera.com)