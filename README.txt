sqlite3 databasename.db
BEGIN;
CREATE TABLE naam(id INTEGER PRIMARY KEY AUTOINCREMENT, lichtwaarde NUMERIC, datum DATE, tijd TIME);
COMMIT;
BEGIN;
INSERT INTO naam (lichtwaarde, datum, tijd) values(724, date('now'), time('now'));
SELECT * FROM naam;
