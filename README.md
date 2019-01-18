# Assignement_3
sqlkod

CREATE TABLE `sqlandjava`.`owners`(
`owner_id`INT(11) NOT NULL,
`person_id`INT(11) NOT NULL,
`car_id`INT(11) NOT NULL,
PRIMARY KEY (`owner_id`));


INSERT INTO `sqlandjava`.`owners`(`owner_id`, `person_id`, `car_id`) VALUES ('1', '2', '3');
INSERT INTO `sqlandjava`.`owners`(`owner_id`, `person_id`, `car_id`) VALUES ('2', '1', '4');
INSERT INTO `sqlandjava`.`owners`(`owner_id`, `person_id`, `car_id`) VALUES ('3', '3', '2');
INSERT INTO `sqlandjava`.`owners`(`owner_id`, `person_id`, `car_id`) VALUES ('4', '4', '1');


CREATE USER user@localhost IDENTIFIED BY 'password';
GRANT SELECT ON sqlandjava.owners TO user@server;




