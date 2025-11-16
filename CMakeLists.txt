idf_component_register (
    SRCS "src/crypto.c"
         "src/wireguard.c"
         "src/wireguardif.c"
         "src/wireguard-platform.c"
         "src/crypto/refc/blake2s.c"
         "src/crypto/refc/chacha20.c"
         "src/crypto/refc/chacha20poly1305.c"
         "src/crypto/refc/poly1305-donna.c"
         "src/esp_wireguard.c"

    INCLUDE_DIRS "include" "src"
    PRIV_INCLUDE_DIRS "src"
    REQUIRES esp_netif lwip mbedtls libsodium
)