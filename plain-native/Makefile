CC=xcrun -sdk iphoneos clang
CFLAGS=-arch arm64
LDFLAGS=-framework Foundation -miphoneos-version-min=12.4 -framework UIKit
# xcrun -sdk iphoneos clang -o prog -arch arm64 prog.m -framework Foundation -framework UIKit -miphoneos-version-min=12.4
# xcrun -sdk iphoneos clang -o prog -arch arm64 prog.m -framework Foundation -miphoneos-version-min=12.4
prog: prog.m
	$(CC) -o $@ $(CFLAGS) $^ $(LDFLAGS)
	ldid -Sprog.ent $@

clean:
	rm -f prog
