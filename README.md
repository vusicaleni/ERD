# ERD
database models
dbms


PLAYER(score, id, level, name)
f.k. level references DIVISION

AMATEUR(score, id) 
f.k. (score, id) references PLAYER

PROFESSIONAL(score, id, matchpoint) 
f.k. (score, id) references PLAYER

DIVISION(level, dos, doe)

MATCH(award, point)

ATTEND(score, id, award, ranking)
f.k. (score, id) references PROFESSIONAL
award references MATCH
