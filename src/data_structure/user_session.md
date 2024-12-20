```mermaid

classDiagram

    class User {
        +String artist_name
        +String artist_type
        +String bio
        +BrandProfile brand
        +String career_level
        +JSON chartmetric_summary
        +JSON cmStatistics
        +String country
        +String[] skills
        +String[] social_media_attitude
        +String user_role
    }

    class BrandProfile {
        +String aspirations
        +String unique_style
        +String values
        +String profile
    }

    class Session {
        +String category
        +String[] keywords
        +String summary
        +TargetAudience intended_target_audience
    }

    class TargetAudience {
        +String demographic
        +String[] interests
        +String[] preferences
    }

    User -- BrandProfile : has
    Session -- TargetAudience : targets

    note for User "Represents Aflow Users"
    note for Session "Represents Recommendable Items"

```
