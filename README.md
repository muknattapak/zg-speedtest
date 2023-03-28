# Dependencies
- docker (docker-engine or docker-desktop)
- docker-compose

# Setup Instruction

## 1. Clone this repository 
```
git clone https://github.com/muknattapak/zg-speedtest
```

## 2. Create persistence storage
```
docker volume create librespeed-speedtest-storage
```

## 3. Build service
```
docker-compose build
```

## 4. Start service
```
docker-compose up -d
```

## 5. Create database
```
docker-compose run create-database
```

# Usage

- Main speed test page is http://localhost:3031/
- Stats page is http://localhost:3031/results/stats.php (default password is `12341234`)
- Database admin ui http://localhost:3032/
