#	$NetBSD: Makefile,v 1.14 2019/03/10 12:14:06 mrg Exp $

LIB=	LLVMIR

.include <bsd.init.mk>

.PATH: ${LLVM_SRCDIR}/lib/IR

TABLEGEN_SRC=		AttributesCompatFunc.td
TABLEGEN_OUTPUT= \
	AttributesCompatFunc.inc|-gen-attrs

.include "${.PARSEDIR}/../../tablegen.mk"

SRCS+=	AsmWriter.cpp \
	Attributes.cpp \
	AutoUpgrade.cpp \
	BasicBlock.cpp \
	Comdat.cpp \
	ConstantFold.cpp \
	ConstantRange.cpp \
	Constants.cpp \
	Core.cpp \
	DataLayout.cpp \
	DebugInfo.cpp \
	DebugInfoMetadata.cpp \
	DebugLoc.cpp \
	DiagnosticHandler.cpp \
	DiagnosticInfo.cpp \
	DiagnosticPrinter.cpp \
	DIBuilder.cpp \
	Dominators.cpp \
	DomTreeUpdater.cpp \
	Function.cpp \
	Globals.cpp \
	GVMaterializer.cpp \
	InlineAsm.cpp \
	Instruction.cpp \
	Instructions.cpp \
	IntrinsicInst.cpp \
	IRBuilder.cpp \
	IRPrintingPasses.cpp \
	LegacyPassManager.cpp \
	LLVMContext.cpp \
	LLVMContextImpl.cpp \
	Mangler.cpp \
	MDBuilder.cpp \
	Metadata.cpp \
	Module.cpp \
	ModuleSummaryIndex.cpp \
	Operator.cpp \
	OptBisect.cpp \
	Pass.cpp \
	PassManager.cpp \
	PassRegistry.cpp \
	ProfileSummary.cpp \
	SafepointIRVerifier.cpp \
	Statepoint.cpp \
	Type.cpp \
	TypeFinder.cpp \
	Use.cpp \
	User.cpp \
	Value.cpp \
	ValueSymbolTable.cpp \
	Verifier.cpp

.if defined(HOSTLIB)
.include <bsd.hostlib.mk>
.else
.include <bsd.lib.mk>
.endif
