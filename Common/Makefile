OBJECTS = AMBEFEC.o AnnouncementUnit.o ArduinoController.o BeaconUnit.o CallsignList.o CCITTChecksum.o CCITTChecksumReverse.o \
	  DStarGMSKDemodulator.o DStarGMSKModulator.o DStarRepeaterConfig.o DStarScrambler.o DummyController.o DVAPController.o \
	  DVMegaController.o DVRPTRV1Controller.o DVRPTRV2Controller.o DVRPTRV3Controller.o DVTOOLFileReader.o DVTOOLFileWriter.o \
	  ExternalController.o FIRFilter.o GatewayProtocolHandler.o GMSKController.o GMSKModem.o GMSKModemLibUsb.o Golay.o \
	  HardwareController.o HeaderData.o K8055Controller.o LogEvent.o Logger.o MMDVMController.o Modem.o OutputQueue.o \
	  RepeaterProtocolHandler.o SerialDataController.o SerialLineController.o SerialPortSelector.o SlowDataDecoder.o SlowDataEncoder.o \
	  SoundCardController.o SoundCardReaderWriter.o SplitController.o TCPReaderWriter.o Timer.o UDPReaderWriter.o \
	  URIUSBController.o Utils.o

all:		Common.a

Common.a:	$(OBJECTS)
		$(AR) rcs Common.a $(OBJECTS)

%.o: %.cpp
		$(CXX) -DwxUSE_GUI=0 $(CFLAGS) -c -o $@ $<

clean:
		$(RM) Common.a *.o *.d *.bak *~

