# $NetBSD: Makefile,v 1.2 2020/06/29 08:54:59 lukem Exp $

KYUA_LIBS=	utils

.include <bsd.init.mk>

TESTSDIR=	${TESTSBASE}/kyua-cli/utils/fs

.PATH:		${SRCDIR}/utils/fs

TESTS_CXX=
.for test in	\
		auto_cleaners_test \
		exceptions_test \
		lua_module_test \
		operations_test \
		path_test
TESTS_CXX+=	${test}
SRCS.${test}=	${test}.cpp
.endfor

.include <bsd.test.mk>
