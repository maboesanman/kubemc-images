FROM itzg/minecraft-server AS minecraft-1.17.1-fabric

ENV VERSION=1.17.1
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

COPY mods/FabricProxy-Lite-1.1.5.jar /mods/
COPY mods/lithium-fabric-mc1.17.1-0.7.5.jar /mods/
COPY mods/phosphor-fabric-mc1.17.x-0.8.0.jar /mods/

COPY config/FabricProxy-Lite.toml /config/

FROM minecraft-1.17.1-fabric AS minecraft-1.17.1-carpet

COPY mods/fabric-carpet-1.17.1-1.4.44+v210714.jar /mods/
