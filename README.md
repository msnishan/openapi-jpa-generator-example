# 🧬 OpenAPI JPA Generator

This project showcases how to generate **JPA entities and relationships** directly from an OpenAPI YAML file using the `openapi-jpa-generator` Gradle plugin.

It demonstrates:
- `@OneToOne` relationships
- `@OneToMany` relationships (bidirectional)
- `@Embedded` and `@Embeddable` classes 
- Few constrains example as well 

---

## 📘 About `example.yaml`

Located at: [`src/main/resources/openapi/example.yaml`](src/main/resources/openapi/example.yaml)

This OpenAPI file defines a sample data model with:

- A `User` entity containing an embedded `Address`
- A `User` ↔ `Order` relationship using `@OneToMany`

---

## ⚙️ How to Generate JPA Code

Make sure the plugin is applied in your `build.gradle.kts`, and then run:

```bash
./gradlew generateOpenApiJpaEntities
```
Generated code will appear in:

```css
generated/src/main/java/
```

## 🛠 Maintained by

**[@msnishan](https://github.com/msnishan)**

