ADD_LIBRARY(ipv6_dhcp SHARED dhcpv6.c dhcpv6_packet.c ppp_ipv6layer.c)
ADD_LIBRARY(ipv6_nd SHARED nd.c ppp_ipv6layer.c)

INSTALL(TARGETS ipv6_dhcp ipv6_nd
	LIBRARY DESTINATION lib${LIB_SUFFIX}/accel-ppp
)

