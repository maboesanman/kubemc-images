FROM itzg/minecraft-server AS fabric-1.18.1

ENV VERSION=1.18.1
ENV USE_AIKAR_FLAGS=TRUE
ENV TYPE=FABRIC
ENV OVERRIDE_SERVER_PROPERTIES=TRUE
ENV ONLINE_MODE=TRUE
ENV REMOVE_OLD_MODS=TRUE
ENV ENABLE_AUTOPAUSE=TRUE
ENV AUTOPAUSE_TIMEOUT_EST=600
ENV MAX_TICK_TIME=-1
ENV TZ=America/Chicago
ENV REPLACE_ENV_DURING_SYNC=TRUE
ENV ENV_VARIABLE_PREFIX=CFG_

COPY mods/fabric-api-0.45.0+1.18.jar /mods/
COPY mods/FabricProxy-Lite-1.1.6.jar /mods/
COPY mods/lithium-fabric-mc1.18.1-0.7.6.jar /mods/
COPY mods/phosphor-fabric-mc1.18.x-0.8.1.jar /mods/

COPY config/FabricProxy-Lite.toml /config/

FROM fabric-1.18.1 AS carpet-1.18.1

COPY mods/fabric-carpet-1.18-1.4.56+v211130.jar /mods/
