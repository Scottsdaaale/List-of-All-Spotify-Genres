# Spotify Genres Database

A comprehensive collection of **6,044 Spotify music genres** sourced from [Every Noise at Once](https://everynoise.com/everynoise1d.cgi?scope=all), available in 12 different formats for seamless integration into any project.

## Overview

This repository contains every Spotify genre available on everynoise.com, formatted for immediate use across different programming languages, databases, and data analysis tools. Whether you're building a music app, conducting genre analysis, or need genre data for machine learning, we've got you covered.

## Available Formats

| Format | File | Description | Size |
|--------|------|-------------|------|
| **JavaScript** | `formats/genres.js` | JS variable assignment | 118KB |
| **JSON** | `formats/genres.json` | Standard JSON array | 118KB |
| **TypeScript** | `formats/genres.ts` | Typed array export | 118KB |
| **CSV** | `formats/genres.csv` | Comma-separated values | 88KB |
| **Plain Text** | `formats/genres.txt` | One genre per line | 88KB |
| **SQL** | `formats/genres.sql` | CREATE TABLE + INSERT statements | 371KB |
| **Python** | `formats/genres.py` | Python list | 130KB |
| **PHP** | `formats/genres.php` | PHP array | 130KB |
| **Ruby** | `formats/genres.rb` | Ruby array | 118KB |
| **Go** | `formats/genres.go` | Go string slice | 112KB |
| **YAML** | `formats/genres.yml` | YAML array | 124KB |
| **XML** | `formats/genres.xml` | XML document | 189KB |
| **Markdown** | `formats/genres.md` | Numbered list | 123KB |

## Quick Start

### JavaScript/Node.js
```javascript
const genres = require('./formats/genres.js');
console.log(genres.length); // 6044
console.log(genres[0]); // "pop"
```

### TypeScript
```typescript
import { genres } from './formats/genres';
const randomGenre: string = genres[Math.floor(Math.random() * genres.length)];
```

### Python
```python
import sys
sys.path.append('formats')
from genres import genres
print(f"Total genres: {len(genres)}")
print(f"First genre: {genres[0]}")
```

### SQL
```bash
# MySQL/MariaDB
mysql -u username -p database_name < formats/genres.sql

# PostgreSQL
psql -U username -d database_name -f formats/genres.sql

# SQLite
sqlite3 mydatabase.db < formats/genres.sql
```

### CSV (Excel, Google Sheets, Pandas)
```python
import pandas as pd
df = pd.read_csv('formats/genres.csv')
```

### PHP
```php
<?php
require 'formats/genres.php';
echo "Total genres: " . count($genres);
```

### Ruby
```ruby
require_relative 'formats/genres'
puts "Total genres: #{genres.length}"
```

### Go
```go
package main
import "fmt"

func main() {
    fmt.Printf("Total genres: %d\n", len(genres))
}
```

## Use Cases

- **Music Applications**: Genre selection dropdowns, filters, and search
- **Data Analysis**: Music trend analysis, genre clustering, recommendation systems
- **Machine Learning**: Training data for genre classification models
- **APIs**: RESTful endpoints serving genre lists
- **Databases**: Pre-populate genre tables for music platforms
- **Testing**: Mock data for music-related unit tests
- **Research**: Academic studies on music categorization

## Genre Examples

The dataset includes a wide variety of genres:
- Mainstream: `pop`, `rock`, `hip hop`, `country`, `edm`
- Regional: `k-pop`, `urbano latino`, `musica mexicana`, `filmi`
- Subgenres: `dance pop`, `melodic rap`, `indie pop`, `tropical house`
- Niche: `baroque brass`, `himene tarava`, `yunnan traditional`

## Data Source

All genres are sourced from [Every Noise at Once](https://everynoise.com/everynoise1d.cgi?scope=all), an ongoing attempt at an algorithmically-generated, readability-adjusted scatter-plot of the musical genre-space, based on data tracked and analyzed by Spotify.

## Stats

- **Total Genres**: 6,044
- **Format Options**: 12
- **Last Updated**: May 2026
- **Data Source**: everynoise.com

## Contributing

Found a missing genre or format you'd like to see? Feel free to open an issue or submit a pull request!

## License

This data is publicly sourced from Every Noise at Once. Please respect Spotify's terms of service when using this data in commercial applications.

## Acknowledgments

- Data sourced from [Every Noise at Once](https://everynoise.com) by Glenn McDonald
- Powered by Spotify's genre classification system
