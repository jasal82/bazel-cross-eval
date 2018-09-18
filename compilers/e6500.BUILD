package(default_visibility = ['//visibility:public'])

filegroup(
  name = 'gcc',
  srcs = [
    'sysroots/x86_64-fslsdk-linux/usr/bin/powerpc64-fsl-linux/powerpc64-fsl-linux-gcc',
  ],
)

filegroup(
  name = 'ar',
  srcs = [
    'sysroots/x86_64-fslsdk-linux/usr/bin/powerpc64-fsl-linux/powerpc64-fsl-linux-ar',
  ],
)

filegroup(
  name = 'ld',
  srcs = [
    'sysroots/x86_64-fslsdk-linux/usr/bin/powerpc64-fsl-linux/powerpc64-fsl-linux-ld',
  ],
)

filegroup(
  name = 'nm',
  srcs = [
    'sysroots/x86_64-fslsdk-linux/usr/bin/powerpc64-fsl-linux/powerpc64-fsl-linux-nm',
  ],
)

filegroup(
  name = 'objcopy',
  srcs = [
    'sysroots/x86_64-fslsdk-linux/usr/bin/powerpc64-fsl-linux/powerpc64-fsl-linux-objcopy',
  ],
)

filegroup(
  name = 'objdump',
  srcs = [
    'sysroots/x86_64-fslsdk-linux/usr/bin/powerpc64-fsl-linux/powerpc64-fsl-linux-objdump',
  ],
)

filegroup(
  name = 'strip',
  srcs = [
    'sysroots/x86_64-fslsdk-linux/usr/bin/powerpc64-fsl-linux/powerpc64-fsl-linux-strip',
  ],
)

filegroup(
  name = 'as',
  srcs = [
    'sysroots/x86_64-fslsdk-linux/usr/bin/powerpc64-fsl-linux/powerpc64-fsl-linux-as',
  ],
)

filegroup(
  name = 'compiler_pieces',
  srcs = glob([
    'sysroots/ppc64e6500-fsl-linux/**',
#    'sysroots/ppc64e6500-fsl-linux/lib/**',
#    'sysroots/ppc64e6500-fsl-linux/lib64/**',
#    'sysroots/ppc64e6500-fsl-linux/usr/lib/**',
#    'sysroots/ppc64e6500-fsl-linux/usr/lib64/**',
    'sysroots/x86_64-fslsdk-linux/**',
  ],
  exclude = [
    'sysroots/x86_64-fslsdk-linux/usr/bin/**',
    'sysroots/ppc64e6500-fsl-linux/etc/ssl/certs/**',
    'sysroots/ppc64e6500-fsl-linux/usr/share/ca-certificates/**',
  ]),
)

filegroup(
  name = 'compiler_components',
  srcs = [
    ':gcc',
    ':ar',
    ':ld',
    ':nm',
    ':objcopy',
    ':objdump',
    ':strip',
    ':as',
  ],
)
