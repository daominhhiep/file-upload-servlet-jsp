create database file_upload;
use file_upload;


CREATE TABLE `employee` (
`id` int(11) primary key ,
 `firstname` varchar(255) NOT NULL,
`lastname` varchar(255) NOT NULL,
`filename` varchar(255) NOT NULL,
`path` varchar(255) NOT NULL,
`added_date` timestamp NOT NULL DEFAULT CURRENT_TIMESTAMP ON UPDATE CURRENT_TIMESTAMP
) ;


INSERT INTO `employee` (`id`, `firstname`, `lastname`, `filename`, `path`, `added_date`) VALUES
(1, 'dharmesh', 'moury', 'dharmesh1.jpg', 'resources\\dharmesh1.jpg', '2018-10-13 18:58:58'),
(2, 'dharmya', 'mourya', 'foodshop.sql', 'resources\\foodshop.sql', '2018-10-13 19:00:21');



CREATE TABLE employee (
                          postId int(11) primary key ,
                          content varchar(255) NOT NULL,
                          images varchar(255) NOT NULL,
                          path varchar(255) NOT NULL,
                          addded_date timestamp NOT NULL DEFAULT CURRENT_TIMESTAMP ON UPDATE CURRENT_TIMESTAMP
) ;