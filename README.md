# setrust
my rust wasm setting so I do not have to start scratch
# Rust 설치
sudo pacman -S rust

# wasm-pack 설치
cargo install wasm-pack

# nginx 설치
sudo pacman -S nginx
sudo systemctl start nginx
sudo systemctl enable nginx

# wasm 폴더 생성
sudo mkdir -p /srv/http/wasm-test
sudo chown -R $USER:$USER /srv/http/wasm-test



# 다운로드한 파일 압축 해제
tar -xzf wasm-setup.tar.gz
cd wasm-setup

# 설치
./install.sh
