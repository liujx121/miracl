include ${FWSRCPATH}/program/makedefs/makedefs
ARMCOMM_OBJDIR=${OBJDIR}/armcomm
UTLDIR=.

# 内部使用的内容
INCDIRPATH =  -I../include

# makedepend 使用的目录
INCDEPPATH = -I${INCDIRPATH}

OBJLIST = \
	${ARMCOMM_OBJDIR}/mrcore.o \
	${ARMCOMM_OBJDIR}/mrarth0.o \
	${ARMCOMM_OBJDIR}/mrarth1.o \
	${ARMCOMM_OBJDIR}/mrarth2.o \
	${ARMCOMM_OBJDIR}/mralloc.o \
	${ARMCOMM_OBJDIR}/mrjack.o   \
	${ARMCOMM_OBJDIR}/mrbits.o   \
	${ARMCOMM_OBJDIR}/mrxgcd.o   \
	${ARMCOMM_OBJDIR}/mrarth3.o   \
	${ARMCOMM_OBJDIR}/mrmonty.o   \
	${ARMCOMM_OBJDIR}/mrsroot.o   \
	${ARMCOMM_OBJDIR}/mrcurve.o   \
	${ARMCOMM_OBJDIR}/mrlucas.o         
SRCLIST = \
	${UTLDIR}/mrcore.c \
	${UTLDIR}/mrarth0.c \
	${UTLDIR}/mrarth1.c \
	${UTLDIR}/mrarth2.c \
	${UTLDIR}/mralloc.c \
	${UTLDIR}/mrjack.c   \
	${UTLDIR}/mrbits.c   \
	${UTLDIR}/mrxgcd.c   \
	${UTLDIR}/mrarth3.c   \
	${UTLDIR}/mrmonty.c   \
	${UTLDIR}/mrsroot.c   \
	${UTLDIR}/mrcurve.c   \
	${UTLDIR}/mrlucas.c      
 
	
all:
	${GM}  ${LIBDIR}/libmiracl.a

#------------------------ Include file dependencies --------------------------
depend:
	@(makedepend -a -p${OBJLIST}/ -o.o -Tlibcomci ${INCDEPPATH} ${LIB_comci_SRCLIST})>/dev/null 2>&1

clean:
	rm -f ${OBJLIST}
	rm -f ${LIBDIR}/libmiracl.a


${LIBDIR}/libmiracl.a : ${OBJLIST} 
	ar -rcs $@ ${OBJLIST} 


#-------------------------逐个编译源文件----------------------------

${ARMCOMM_OBJDIR}/mrcore.o : ${UTLDIR}/mrcore.c
	${SOCXX} -c ${SOCXXFLAGS} ${INCDIRPATH} ${CXXMTFLAGS} $< -o $@

${ARMCOMM_OBJDIR}/mrarth0.o : ${UTLDIR}/mrarth0.c
	${SOCXX} -c ${SOCXXFLAGS} ${INCDIRPATH} ${CXXMTFLAGS} $< -o $@

${ARMCOMM_OBJDIR}/mrarth1.o : ${UTLDIR}/mrarth1.c
	${SOCXX} -c ${SOCXXFLAGS} ${INCDIRPATH} ${CXXMTFLAGS} $< -o $@

${ARMCOMM_OBJDIR}/mrarth2.o : ${UTLDIR}/mrarth2.c
	${SOCXX} -c ${SOCXXFLAGS} ${INCDIRPATH} ${CXXMTFLAGS} $< -o $@

${ARMCOMM_OBJDIR}/mralloc.o : ${UTLDIR}/mralloc.c
	${SOCXX} -c ${SOCXXFLAGS} ${INCDIRPATH} ${CXXMTFLAGS} $< -o $@

${ARMCOMM_OBJDIR}/mrjack.o : ${UTLDIR}/mrjack.c
	${SOCXX} -c ${SOCXXFLAGS} ${INCDIRPATH} ${CXXMTFLAGS} $< -o $@

${ARMCOMM_OBJDIR}/mrbits.o : ${UTLDIR}/mrbits.c
	${SOCXX} -c ${SOCXXFLAGS} ${INCDIRPATH} ${CXXMTFLAGS} $< -o $@

${ARMCOMM_OBJDIR}/mrxgcd.o : ${UTLDIR}/mrxgcd.c
	${SOCXX} -c ${SOCXXFLAGS} ${INCDIRPATH} ${CXXMTFLAGS} $< -o $@

${ARMCOMM_OBJDIR}/mrarth3.o : ${UTLDIR}/mrarth3.c
	${SOCXX} -c ${SOCXXFLAGS} ${INCDIRPATH} ${CXXMTFLAGS} $< -o $@

${ARMCOMM_OBJDIR}/mrmonty.o : ${UTLDIR}/mrmonty.c
	${SOCXX} -c ${SOCXXFLAGS} ${INCDIRPATH} ${CXXMTFLAGS} $< -o $@

${ARMCOMM_OBJDIR}/mrsroot.o : ${UTLDIR}/mrsroot.c
	${SOCXX} -c ${SOCXXFLAGS} ${INCDIRPATH} ${CXXMTFLAGS} $< -o $@

${ARMCOMM_OBJDIR}/mrcurve.o : ${UTLDIR}/mrcurve.c
	${SOCXX} -c ${SOCXXFLAGS} ${INCDIRPATH} ${CXXMTFLAGS} $< -o $@

${ARMCOMM_OBJDIR}/mrlucas.o : ${UTLDIR}/mrlucas.c
	${SOCXX} -c ${SOCXXFLAGS} ${INCDIRPATH} ${CXXMTFLAGS} $< -o $@






# DO NOT DELETE THIS LINE -- make depend depends on it.
