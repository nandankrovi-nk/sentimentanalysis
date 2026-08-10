# Data Dictionary

| Column | Description |
|---|---|
| `review_id` | Unique identifier for a review |
| `product_name` | Product model/name reviewed |
| `product_id` | Product identifier / ASIN |
| `title` | Review title |
| `author` | Reviewer name or alias |
| `rating` | Star rating, typically 1–5 |
| `content` | Full review text |
| `timestamp` | Date/time review was posted |
| `profile_id` | Reviewer profile identifier |
| `is_verified` | Whether purchase was verified |
| `helpful_count` | Number of helpful votes |
| `product_attributes` | Product variant attributes such as color/style |
| `clean_content` | Cleaned text used for NLP |
| `review_length` | Character count after cleaning |
| `word_count` | Number of words after cleaning |
| `polarity` | TextBlob sentiment polarity from -1 to +1 |
| `subjectivity` | TextBlob subjectivity from 0 to 1 |
| `sentiment` | Positive, Neutral, or Negative label |
