// AVIOCTRL Message Type
typedef enum 
{
//	IOTYPE_USER_IPCAM_START 					= 0x01FF,
	IOTYPE_USER_IPCAM_STOP	 					= 0x02FF,
	IOTYPE_USER_IPCAM_AUDIOSTART 				= 0x0300,
	IOTYPE_USER_IPCAM_AUDIOSTOP 				= 0x0301,

//	IOTYPE_USER_IPCAM_SPEAKERSTART 				= 0x0350,
//	IOTYPE_USER_IPCAM_SPEAKERSTOP 				= 0x0351,

	IOTYPE_USER_IPCAM_SETSTREAMCTRL_REQ			= 0x0320,
	IOTYPE_USER_IPCAM_SETSTREAMCTRL_RESP		= 0x0321,
	IOTYPE_USER_IPCAM_GETSTREAMCTRL_REQ			= 0x0322,
	IOTYPE_USER_IPCAM_GETSTREAMCTRL_RESP		= 0x0323,

	IOTYPE_USER_IPCAM_SETMOTIONDETECT_REQ		= 0x0324,
	IOTYPE_USER_IPCAM_SETMOTIONDETECT_RESP		= 0x0325,
	IOTYPE_USER_IPCAM_GETMOTIONDETECT_REQ		= 0x0326,
	IOTYPE_USER_IPCAM_GETMOTIONDETECT_RESP		= 0x0327,
	
	IOTYPE_USER_IPCAM_GETSUPPORTSTREAM_REQ		= 0x0328,	// Get Support Stream
	IOTYPE_USER_IPCAM_GETSUPPORTSTREAM_RESP		= 0x0329,	

	IOTYPE_USER_IPCAM_DEVINFO_REQ				= 0x0330,
	IOTYPE_USER_IPCAM_DEVINFO_RESP				= 0x0331,

	IOTYPE_USER_IPCAM_SETPASSWORD_REQ			= 0x0332,
	IOTYPE_USER_IPCAM_SETPASSWORD_RESP			= 0x0333,

	IOTYPE_USER_IPCAM_LISTWIFIAP_REQ			= 0x0340,
	IOTYPE_USER_IPCAM_LISTWIFIAP_RESP			= 0x0341,
	IOTYPE_USER_IPCAM_SETWIFI_REQ				= 0x0342,
	IOTYPE_USER_IPCAM_SETWIFI_RESP				= 0x0343,
	IOTYPE_USER_IPCAM_GETWIFI_REQ				= 0x0344,
	IOTYPE_USER_IPCAM_GETWIFI_RESP				= 0x0345,
	IOTYPE_USER_IPCAM_SETWIFI_REQ_2				= 0x0346,
	IOTYPE_USER_IPCAM_GETWIFI_RESP_2			= 0x0347,

	IOTYPE_USER_IPCAM_SETRECORD_REQ				= 0x0310,
	IOTYPE_USER_IPCAM_SETRECORD_RESP			= 0x0311,
	IOTYPE_USER_IPCAM_GETRECORD_REQ				= 0x0312,
	IOTYPE_USER_IPCAM_GETRECORD_RESP			= 0x0313,

	IOTYPE_USER_IPCAM_SETRCD_DURATION_REQ		= 0x0314,
	IOTYPE_USER_IPCAM_SETRCD_DURATION_RESP  	= 0x0315,
	IOTYPE_USER_IPCAM_GETRCD_DURATION_REQ		= 0x0316,
	IOTYPE_USER_IPCAM_GETRCD_DURATION_RESP  	= 0x0317,

	IOTYPE_USER_IPCAM_LISTEVENT_REQ				= 0x0318,
	IOTYPE_USER_IPCAM_LISTEVENT_RESP			= 0x0319,
	
	IOTYPE_USER_IPCAM_RECORD_PLAYCONTROL 		= 0x031A,
	IOTYPE_USER_IPCAM_RECORD_PLAYCONTROL_RESP 	= 0x031B,
	
	IOTYPE_USER_IPCAM_GETAUDIOOUTFORMAT_REQ		= 0x032A,
	IOTYPE_USER_IPCAM_GETAUDIOOUTFORMAT_RESP	= 0x032B,

	IOTYPE_USER_IPCAM_GET_EVENTCONFIG_REQ		= 0x0400,	// Get Event Config Msg Request
	IOTYPE_USER_IPCAM_GET_EVENTCONFIG_RESP		= 0x0401,	// Get Event Config Msg Response
	IOTYPE_USER_IPCAM_SET_EVENTCONFIG_REQ		= 0x0402,	// Set Event Config Msg req
	IOTYPE_USER_IPCAM_SET_EVENTCONFIG_RESP		= 0x0403,	// Set Event Config Msg resp

	IOTYPE_USER_IPCAM_SET_ENVIRONMENT_REQ		= 0x0360,
	IOTYPE_USER_IPCAM_SET_ENVIRONMENT_RESP		= 0x0361,
	IOTYPE_USER_IPCAM_GET_ENVIRONMENT_REQ		= 0x0362,
	IOTYPE_USER_IPCAM_GET_ENVIRONMENT_RESP		= 0x0363,
	
	IOTYPE_USER_IPCAM_SET_VIDEOMODE_REQ			= 0x0370,	// Set Video Flip Mode
	IOTYPE_USER_IPCAM_SET_VIDEOMODE_RESP		= 0x0371,
	IOTYPE_USER_IPCAM_GET_VIDEOMODE_REQ			= 0x0372,	// Get Video Flip Mode
	IOTYPE_USER_IPCAM_GET_VIDEOMODE_RESP		= 0x0373,
	
	IOTYPE_USER_IPCAM_FORMATEXTSTORAGE_REQ		= 0x0380,	// Format external storage
	IOTYPE_USER_IPCAM_FORMATEXTSTORAGE_RESP		= 0x0381,	
	
	IOTYPE_USER_IPCAM_PTZ_COMMAND				= 0x1001,	// P2P PTZ Command Msg

	IOTYPE_USER_IPCAM_EVENT_REPORT				= 0x1FFF,	// Device Event Report Msg
	IOTYPE_USER_IPCAM_RECEIVE_FIRST_IFRAME		= 0x1002,	// Send from client, used to talk to device that
															// client had received the first I frame
	
	IOTYPE_USER_IPCAM_GET_FLOWINFO_REQ			= 0x0390,
	IOTYPE_USER_IPCAM_GET_FLOWINFO_RESP			= 0x0391,
	IOTYPE_USER_IPCAM_CURRENT_FLOWINFO			= 0x0392,
	
	IOTYPE_USER_IPCAM_GET_TIMEZONE_REQ          = 0x3A0,
	IOTYPE_USER_IPCAM_GET_TIMEZONE_RESP         = 0x3A1,
	IOTYPE_USER_IPCAM_SET_TIMEZONE_REQ          = 0x3B0,
	IOTYPE_USER_IPCAM_SET_TIMEZONE_RESP         = 0x3B1,

	IOTYPE_USER_IPCAM_SET_VSAASINFO_REQ		    = 0x0410,
	IOTYPE_USER_IPCAM_SET_VSAASINFO_RESP        = 0x0411,
    

    // dropbox support
    IOTYPE_USER_IPCAM_GET_SAVE_DROPBOX_REQ      = 0x500,
    IOTYPE_USER_IPCAM_GET_SAVE_DROPBOX_RESP     = 0x501,
    IOTYPE_USER_IPCAM_SET_SAVE_DROPBOX_REQ      = 0x502,
    IOTYPE_USER_IPCAM_SET_SAVE_DROPBOX_RESP     = 0x503,

    // ptz preset
	IOTYPE_HICHIP_CRUISE_START                  = 0x600,
	IOTYPE_HICHIP_CRUISE_STOP                   = 0x601,

	IOTYPE_USER_IPCAM_SETPRESET_REQ             = 0x440,
	IOTYPE_USER_IPCAM_SETPRESET_RESP            = 0x441,
	IOTYPE_USER_IPCAM_GETPRESET_REQ             = 0x442,
	IOTYPE_USER_IPCAM_GETPRESET_RESP            = 0x443,

	IOTYPE_USER_IPCAM_DOOROPEN_REQ              = 0x800,
	IOTYPE_USER_IPCAM_DOOROPEN_RESP             = 0x801,

	// for IP02/IPC product
	IOTYPE_USER_IPCAM_SET_PUSH_REQ              = 0x802,
	IOTYPE_USER_IPCAM_SET_PUSH_RESP             = 0x803,

	IOTYPE_USER_IPCAM_DEL_PUSH_REQ              = 0x804,
	IOTYPE_USER_IPCAM_DEL_PUSH_RESP             = 0x805,

	IOTYPE_USER_IPCAM_SET_MDP_REQ				= 0x806,
	IOTYPE_USER_IPCAM_SET_MDP_RESP				= 0x807,
	IOTYPE_USER_IPCAM_GET_MDP_REQ				= 0x808,
	IOTYPE_USER_IPCAM_GET_MDP_RESP				= 0x809,

	IOTYPE_USER_IPCAM_DOORPASS_REQ              = 0x812,
	IOTYPE_USER_IPCAM_DOORPASS_RESP             = 0x813,

	IOTYPE_USER_IPCAM_SET_DEVICETIME_REQ        = 0x816,
	IOTYPE_USER_IPCAM_SET_DEVICETIME_RESP       = 0x817,

	IOTYPE_USER_IPCAM_ALARMING_REQ				= 0x850,
	IOTYPE_USER_IPCAM_ALARMING_RESP				= 0x851,

    IOTYPE_USER_IPCAM_SET_SYSTEM_REQ			= 0x852,
    IOTYPE_USER_IPCAM_SET_SYSTEM_RESP			= 0x853,

    IOTYPE_USER_IPCAM_GET_SYSTEM_REQ			= 0x854,
	IOTYPE_USER_IPCAM_GET_SYSTEM_RESP			= 0x855,

    IOTYPE_USER_IPCAM_GET_SDCARD_REQ            = 0x856,
    IOTYPE_USER_IPCAM_GET_SDCARD_RESP           = 0x857,

    IOTYPE_USER_IPCAM_GET_OSD_REQ               = 0x858,
    IOTYPE_USER_IPCAM_GET_OSD_RESP              = 0x859,
    IOTYPE_USER_IPCAM_SET_OSD_REQ               = 0x860,
    IOTYPE_USER_IPCAM_SET_OSD_RESP              = 0x861,
	IOTYPE_USER_IPCAM_SET_433_REQ				= 0x862,
	IOTYPE_USER_IPCAM_SET_433_RESP				= 0x863,
	IOTYPE_USER_IPCAM_GET_433_REQ				= 0x864,
	IOTYPE_USER_IPCAM_GET_433_RESP				= 0x865,
	IOTYPE_USER_IPCAM_CFG_433_REQ				= 0x866,
	IOTYPE_USER_IPCAM_CFG_433_RESP				= 0x867,
	IOTYPE_USER_IPCAM_DEL_433_REQ				= 0x868,
	IOTYPE_USER_IPCAM_DEL_433_RESP				= 0x869,
	IOTYPE_USER_IPCAM_CFG_433_EXIT_REQ			= 0x870,
	IOTYPE_USER_IPCAM_CFG_433_EXIT_RESP			= 0x871,

    IOTYPE_USER_IPCAM_GET_CAPACITY_REQ          = 0x880,
    IOTYPE_USER_IPCAM_GET_CAPACITY_RESP         = 0x881,

    IOTYPE_USER_IPCAM_GET_MD_ALAM_REQ           = 0x882,
    IOTYPE_USER_IPCAM_GET_MD_ALAM_RESP          = 0x883,
    IOTYPE_USER_IPCAM_SET_MD_ALAM_REQ           = 0x884,
    IOTYPE_USER_IPCAM_SET_MD_ALAM_RESP          = 0x885,

    IOTYPE_USER_IPCAM_GET_AUDIO_REQ             = 0x886,
    IOTYPE_USER_IPCAM_GET_AUDIO_RESP            = 0x887,
    IOTYPE_USER_IPCAM_SET_AUDIO_REQ             = 0x888,
    IOTYPE_USER_IPCAM_SET_AUDIO_RESP            = 0x889,

    IOTYPE_USER_IPCAM_UPDATE_REQ                = 0x88a,
    IOTYPE_USER_IPCAM_UPDATE_RESP               = 0x88b,
    IOTYPE_USER_IPCAM_UPDATE_PROG_REQ           = 0x88c,
    IOTYPE_USER_IPCAM_UPDATE_PROG_RESP          = 0x88d,
  
    IOTYPE_USER_IPCAM_SHELL_REQ                 = 0x88e,    
    IOTYPE_USER_IPCAM_SHELL_RESP                = 0x88f,
    IOTYPE_USER_IPCAM_HEARTBEAT_REQ             = 0x890,
    IOTYPE_USER_IPCAM_HEARTBEAT_RESP            = 0x891,

	IOTYPE_USER_IPCAM_SEND_META_START           = 0x200,
    IOTYPE_USER_IPCAM_SEND_META_STOP            = 0x201,
	
    IOTYPE_USER_IPCAM_PUSH_STREAMING_START      = 0x210,
	IOTYPE_USER_IPCAM_PUSH_STREAMING_START_RESP = 0x211,
    IOTYPE_USER_IPCAM_PUSH_STREAMING_FINISH     = 0x212,
	IOTYPE_USER_IPCAM_PUSH_STREAMING_FINISH_RESP= 0x213,
	IOTYPE_USER_IPCAM_PUSH_STREAMING_CLOSE      = 0x214,

	// define for pixsee
	// TUTK Default Commands, app (client) to device (server)
	IOTYPE_USER_IPCAM_START 							= 0x01FF,		// struct SMsgAVIoctrlAVStream;
	IOTYPE_USER_IPCAM_STOP								= 0x02FF,		// struct SMsgAVIoctrlAVStream;
	IOTYPE_USER_IPCAM_AUDIOSTART						= 0x0300,		// struct SMsgAVIoctrlAVStream;
	IOTYPE_USER_IPCAM_AUDIOSTOP							= 0x0301,		// struct SMsgAVIoctrlAVStream;
	IOTYPE_USER_IPCAM_RECORD_PLAYCONTROL				= 0x031A,		// struct SMsgAVIoctrlPlayRecord;
	IOTYPE_USER_IPCAM_DEVINFO_REQ						= 0x0300,
	IOTYPE_USER_IPCAM_DEVINFO_RESP						= 0x0331,		// struct SMsgAVIoctrlDeviceInfoResp;
	IOTYPE_USER_IPCAM_GETWIFI_REQ 						= 0x0344,
	IOTYPE_USER_IPCAM_GETWIFI_RESP 						= 0x0345,		// struct SMsgAVIoctrlSetWifiReq;
	IOTYPE_USER_IPCAM_SPEAKERSTART						= 0x0350,		// struct SMsgAVIoctrlAVStream;
	IOTYPE_USER_IPCAM_SPEAKERSTOP						= 0x0351,
	IOTYPE_USER_IPCAM_GET_TIMEZONE_REQ					= 0x03A0,
	IOTYPE_USER_IPCAM_GET_TIMEZONE_RESP					= 0x03A1,
	IOTYPE_USER_IPCAM_SET_TIMEZONE_REQ					= 0x03B0,
	IOTYPE_USER_IPCAM_SET_TIMEZONE_RESP					= 0x03B1,		// struct SMsgAVIoctrlTimeZone; 
	IOTYPE_USER_IPCAM_SET_VSAASINFO_REQ					= 0x0410,		// struct SMsgAVIoctrlSetVsaasInfoReq;
	IOTYPE_USER_IPCAM_SET_VSAASINFO_RESP				= 0x0411,		// struct SMsgAVIoctrlSetVsaasInfoResp;
	// end of TUTK Default Commands
	IOTYPE_USER_IPCAM_CEI_MUSIC_PLAYCONTROL_REQ			= 0x1100,		// struct SMsgAVIoctrlPlayMusic;
	IOTYPE_USER_IPCAM_CEI_MUSIC_PLAYCONTROL_RESP		= 0x1101,		// struct SMsgAVIoctrlPlayMusicResp;
	IOTYPE_USER_IPCAM_CEI_SETSTREAMCTRL_REQ				= 0x1200,		// struct SMsgAVIoctrlCEISetStreamCtrl;
	IOTYPE_USER_IPCAM_CEI_RECORDQUERY_REQ				= 0x1210,
	IOTYPE_USER_IPCAM_CEI_RECORDQUERY_RESP				= 0x1201,		// struct SMsgAVIoctrlRecordQueryResp;
	IOTYPE_USER_IPCAM_CEI_SETTEMHUM_REQ_NEW				= 0x1300,		// struct SMsgAVIoctrlCEISetTemperatureHumidity;
	IOTYPE_USER_IPCAM_CEI_GETTEMHUM_REQ_NEW				= 0x1301,
	IOTYPE_USER_IPCAM_CEI_GETTEMHUM_RESP_NEW			= 0x1302,		// struct SMsgAVIoctrlCEISetTemperatureHumidity;
	IOTYPE_USER_IPCAM_CEI_GETCURRENTTEMHUM_REQ_NEW		= 0x1303,
	IOTYPE_USER_IPCAM_CEI_GETCURRENTTEMHUM_RESP_NEW		= 0x1304,		// struct SMsgAVIoctrlCEIGetCurrentTemperatureHumidity;
	IOTYPE_USER_IPCAM_CEI_SETDANGERZOOM_REQ_NEW			= 0x1400,		// struct SMsgAVIoctrlCEISetDangerZoom;
	IOTYPE_USER_IPCAM_CEI_GETDANGERZOOM_REQ_NEW			= 0x1401,
	IOTYPE_USER_IPCAM_CEI_GETDANGERZOOM_RESP_NEW		= 0x1402,		// struct SMsgAVIoctrlCEISetDangerZoom;
	IOTYPE_USER_IPCAM_CEI_GETDEVICEOOBESTATUS_REQ_NEW 	= 0x1500,
	IOTYPE_USER_IPCAM_CEI_GETDEVICEOOBESTATUS_RESP_NEW	= 0x1501,		// 1 (means device is ready to go) or 
																		// 0 (means device status is not ready)
	IOTYPE_USER_IPCAM_CEI_SET_INFANT_ID_REQ_NEW			= 0x1600,		// no need anymore
	IOTYPE_USER_IPCAM_CEI_SET_INFANT_ID_RESP			= 0x1601,		// no need anymore
	IOTYPE_USER_IPCAM_CEI_GETCRY_REQ_NEW				= 0x1700,		// no need anymore
	IOTYPE_USER_IPCAM_CEI_GETCRY_RESP_NEW				= 0x1701,		// no need anymore
	IOTYPE_USER_IPCAM_CEI_SETCRYMODE_REQ_NEW			= 0x1702,		// struct SMsgAVIoctrlCEISetCryModeReq;
	IOTYPE_USER_IPCAM_CEI_GETCRYMODE_REQ				= 0x1703,		// struct SMsgAVIoctrlCEIGetCryModeResp;
	IOTYPE_USER_IPCAM_CEI_SETCRYMUSIC_REQ				= 0x1705,		// struct SMsgAVIoctrlCEISetCryMusicReq;
	IOTYPE_USER_IPCAM_CEI_SETCRYMUSIC_FILE_REQ			= 0x1706,		// struct SMsgAVIoctrlCEISetCryMusicFileReq;
	IOTYPE_USER_IPCAM_CEI_SETCRYMUSIC_FILE_RESP			= 0x1707,		// struct SMsgAVIoctrlCEISetCryMusicFileResp;
	IOTYPE_USER_IPCAM_CEI_GETCRYMUSIC_FILE_REQ			= 0x1708, 		// struct SMsgAVIoctrlCEIGetCryMusicFileReq;
	IOTYPE_USER_IPCAM_CEI_GETCRYMUSIC_FILE_RESP			= 0x1709,		// struct SMsgAVIoctrlCEIGetCryMusicFileResp;
	IOTYPE_USER_IPCAM_CEI_GETSOOTHINGMODE_REQ			= 0x170A,
	IOTYPE_USER_IPCAM_CEI_GETSOOTHINGMODE_RESP			= 0x170B,		// struct SMsgAVIoctrlSoothingMode;
	IOTYPE_USER_IPCAM_CEI_SETLEDCTRL_REQ_NEW			= 0x1800,		// struct SMsgAVIoctrlCEISetLEDReq;
	IOTYPE_USER_IPCAM_CEI_GETLEDCTRL_REQ				= 0x1801,
	IOTYPE_USER_IPCAM_CEI_GETLEDCTRL_RESP				= 0x1802,		// struct SMsgAVIoctrlCEIGetLedModeResp;
	IOTYPE_USER_IPCAM_CEI_SETNIGHTMODECTRL_REQ_NEW		= 0x1810,		// struct SMsgAVIoctrlCEISetNightModeReq;
	IOTYPE_USER_IPCAM_CEI_GETNIGHTMODECTRL_REQ			= 0x1811,
	IOTYPE_USER_IPCAM_CEI_GETNIGHTMODECTRL_RESP			= 0x1812,		// struct SMsgAVIoctrlCEIGetNightModeResp;
	IOTYPE_USER_IPCAM_CEI_SETNOTIFYCTRL_REQ				= 0x1820,		// struct SMsgAVIoctrlNotifyControlReq;
	IOTYPE_USER_IPCAM_CEI_GETNOTIFYCTRL_REQ				= 0x1821,
	IOTYPE_USER_IPCAM_CEI_GETNOTIFYCTRL_RESP			= 0x1822,		// struct SMsgAVIoctrlNotifyControlResp;
	IOTYPE_USER_IPCAM_CEI_2WAYSTATUS_REQ				= 0x1830,
	IOTYPE_USER_IPCAM_CEI_2WAYSTATUS_RESP				= 0x1831,		// struct SMsgAVIoctrlStatus;
	IOTYPE_USER_IPCAM_CEI_2WAYMIC_REQ					= 0x1832,		// struct SMsgAVIoctrlMicReq;
	IOTYPE_USER_IPCAM_CEI_FACTORYRESET_REQ				= 0x1900,		// struct SMsgAVIoctrlCEIFactoryResetReq;
	IOTYPE_USER_IPCAM_CEI_FACTORYRESET_RESP				= 0x1901,		// struct SMsgAVIoctrlCEIFactoryResetResp;
	IOTYPE_USER_IPCAM_STARTFWUPGRADE_REQ				= 0x1920,
	IOTYPE_USER_IPCAM_STARTFWUPGRADE_RESP				= 0x1921,
	IOTYPE_USER_IPCAM_OTA_READY_REQ						= 0x1922,
	IOTYPE_USER_IPCAM_OTA_READY_RESP					= 0x1923,		// struct SMsgAVIoctrlOtaReadyResp;
	IOTYPE_USER_IPCAM_OTAINFO_REQ						= 0x1924,
	IOTYPE_USER_IPCAM_OTAINFO_RESP						= 0x1925,		// struct SMsgAVIoctrlOtaInfoResp;
	
	
	// end of define for pixsee

    IOTYPE_USER_CMD_MAX
}ENUM_AVIOCTRL_MSGTYPE;