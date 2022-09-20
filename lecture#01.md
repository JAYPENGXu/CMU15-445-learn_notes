一、关系模型

1. Relation model : 
2. Primary keys
3. Foreign keys

多对多的时候拿一个中间表做映射

3. DML（data manipulation languages）

-- Procedural

-- Non-Procedural

```sql
Select  
Projection
Union
Intersection
Difference
Product
Join
```

4. Relational Algebra : select

Choose a subset of the tuples from a  relation that satisfies a selection  predicate.

```sql
SELECT * FROM R
WHERE a_id='a2' AND b_id=>102;
```

5. Relational Algebra : Projection

Generate a relation with tuples that  contains only the specified attributes.(1 Can rearrange attributes’ ordering;2 Can manipulate the values)

```sql
SELECT b_id-100, a_id
	FROM R WHERE a_id = 'a2';
```

6. Relational Algebra: Union

Generate a relation that contains all  tuples that appear in either only one  or both input relations.

```sql
(SELECT * FROM R) UNION ALL (SELECT * FROM S);
```

7. Relational Algebra: Intersection

Generate a relation that contains only  the tuples that appear in both of the  input relations.

```sql
(SELECT * FROM R) INTERSECT (SELECT * FROM S);
```

8. Relational Algebra : Difference

Generate a relation that contains only  the tuples that appear in the first and  not the second of the input relations.

```sql
(SELECT * FROM R) EXCEPT (SELECT * FROM S);
```

9. Relational Algebra: Product

Generate a relation that contains all  possible combinations of tuples from  the input relations.

```sql
SELECT * FROM R CROSS JOIN S;
SELECT * FROM R, S;
```

10. Relational Algebra: Join

Generate a relation that contains all  tuples that are a combination of two  tuples (one from each input relation)  with a common value(s) for one or  more attributes.

```sql
SELECT * FROM R NATURAL JOIN S;
```

