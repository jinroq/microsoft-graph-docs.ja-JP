# <a name="enroll-devices-for-management-in-intune"></a><span data-ttu-id="4361f-101">Intune における管理用にデバイスを登録する</span><span class="sxs-lookup"><span data-stu-id="4361f-101">Enroll devices for management in InTune</span></span>

> <span data-ttu-id="4361f-102">**注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://www.microsoft.com/ja-JP/cloud-platform/microsoft-intune-pricing)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="4361f-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://www.microsoft.com/ja-JP/cloud-platform/microsoft-intune-pricing) by the customer.</span></span>

<span data-ttu-id="4361f-103">デバイス (Windows PC を含む) を登録して、Microsoft Intune でモバイル デバイス管理 (MDM) を有効にすることができます。</span><span class="sxs-lookup"><span data-stu-id="4361f-103">You can enroll devices, including Windows PCs, to enable mobile device management (MDM) with Microsoft Intune.</span></span> <span data-ttu-id="4361f-104">このトピックでは、Intune 管理における、いくつかのモバイル デバイスの登録方法について説明します。</span><span class="sxs-lookup"><span data-stu-id="4361f-104">This topic describes different ways to enroll mobile devices in Intune management.</span></span> <span data-ttu-id="4361f-105">デバイスを登録する方法は、デバイスの種類、所有権、必要な管理のレベルによって異なります。</span><span class="sxs-lookup"><span data-stu-id="4361f-105">The way you enroll your devices depends on the device type, ownership, and the level of management that's needed.</span></span> <span data-ttu-id="4361f-106">"Bring Your Own Device" (BYOD) の登録により、ユーザーは、個人の電話、タブレット、PC を登録することができます。</span><span class="sxs-lookup"><span data-stu-id="4361f-106">"Bring your own device" (BYOD) enrollment lets users enroll their personal phones, tablets, or PCs.</span></span> <span data-ttu-id="4361f-107">会社所有のデバイス (COD) の登録により、リモートワイプ、共有デバイス、デバイスのユーザー アフィニティなどの管理シナリオが可能になります。</span><span class="sxs-lookup"><span data-stu-id="4361f-107">Corporate-owned device (COD) enrollment enables management scenarios like remote wipe, shared devices, or user affinity for a device.</span></span>

<span data-ttu-id="4361f-108">次の Graph リソースを使用して、Intune での登録を管理できます。</span><span class="sxs-lookup"><span data-stu-id="4361f-108">The following Graph resources are available to manage enrollment in Intune:</span></span>

- [<span data-ttu-id="4361f-109">Apple プッシュ通知証明書</span><span class="sxs-lookup"><span data-stu-id="4361f-109">Apple push notification certificate</span></span>](intune_devices_applepushnotificationcertificate.md)
- [<span data-ttu-id="4361f-110">監査アクター</span><span class="sxs-lookup"><span data-stu-id="4361f-110">Audit actor</span></span>](intune_auditing_auditactor.md)
- [<span data-ttu-id="4361f-111">監査イベント</span><span class="sxs-lookup"><span data-stu-id="4361f-111">Audit event</span></span>](intune_auditing_auditevent.md)
- [<span data-ttu-id="4361f-112">監査のプロパティ</span><span class="sxs-lookup"><span data-stu-id="4361f-112">Audit property</span></span>](intune_auditing_auditproperty.md)
- [<span data-ttu-id="4361f-113">監査のリソース</span><span class="sxs-lookup"><span data-stu-id="4361f-113">Audit resource</span></span>](intune_auditing_auditresource.md)
- [<span data-ttu-id="4361f-114">構成マネージャーのクライアントに対応した機能</span><span class="sxs-lookup"><span data-stu-id="4361f-114">Configuration manager client enabled features</span></span>](intune_devices_configurationmanagerclientenabledfeatures.md)
- [<span data-ttu-id="4361f-115">共有の Apple デバイスのアクションの結果からユーザーを削除する</span><span class="sxs-lookup"><span data-stu-id="4361f-115">Delete user from shared Apple device action result</span></span>](intune_devices_deleteuserfromsharedappledeviceactionresult.md)
- [<span data-ttu-id="4361f-116">検出されたアプリ</span><span class="sxs-lookup"><span data-stu-id="4361f-116">Detected app</span></span>](intune_devices_detectedapp.md)
- [<span data-ttu-id="4361f-117">デバイスのアクションの結果</span><span class="sxs-lookup"><span data-stu-id="4361f-117">Device action result</span></span>](intune_devices_deviceactionresult.md)
- [<span data-ttu-id="4361f-118">デバイス カテゴリ</span><span class="sxs-lookup"><span data-stu-id="4361f-118">Device category</span></span>](intune_devices_devicecategory.md)
- [<span data-ttu-id="4361f-119">デバイスの Exchange アクセス状態の要約</span><span class="sxs-lookup"><span data-stu-id="4361f-119">Device exchange access state summary</span></span>](intune_devices_deviceexchangeaccessstatesummary.md)
- [<span data-ttu-id="4361f-120">デバイスの位置情報</span><span class="sxs-lookup"><span data-stu-id="4361f-120">Device geolocation</span></span>](intune_devices_devicegeolocation.md)
- [<span data-ttu-id="4361f-121">デバイスの正常性構成証明の状態</span><span class="sxs-lookup"><span data-stu-id="4361f-121">Device health attestation state</span></span>](intune_devices_devicehealthattestationstate.md)
- [<span data-ttu-id="4361f-122">デバイス管理のトラブルシューティング イベント</span><span class="sxs-lookup"><span data-stu-id="4361f-122">Device management troubleshooting event</span></span>](intune_troubleshooting_devicemanagementtroubleshootingevent.md)
- [<span data-ttu-id="4361f-123">デバイスの管理</span><span class="sxs-lookup"><span data-stu-id="4361f-123">Device management</span></span>](intune_devices_devicemanagement.md)
- [<span data-ttu-id="4361f-124">デバイスの管理</span><span class="sxs-lookup"><span data-stu-id="4361f-124">Device management</span></span>](intune_endpointprotection_devicemanagement.md)
- [<span data-ttu-id="4361f-125">デバイスの管理</span><span class="sxs-lookup"><span data-stu-id="4361f-125">Device management</span></span>](intune_notification_devicemanagement.md)
- [<span data-ttu-id="4361f-126">デバイスの管理</span><span class="sxs-lookup"><span data-stu-id="4361f-126">Device management</span></span>](intune_remoteassistance_devicemanagement.md)
- [<span data-ttu-id="4361f-127">デバイスの管理</span><span class="sxs-lookup"><span data-stu-id="4361f-127">Device management</span></span>](intune_troubleshooting_devicemanagement.md)
- [<span data-ttu-id="4361f-128">デバイスの管理</span><span class="sxs-lookup"><span data-stu-id="4361f-128">Device management</span></span>](intune_auditing_devicemanagement.md)
- [<span data-ttu-id="4361f-129">デバイスのオペレーティング システムの概要</span><span class="sxs-lookup"><span data-stu-id="4361f-129">Device operating system summary</span></span>](intune_devices_deviceoperatingsystemsummary.md)
- [<span data-ttu-id="4361f-130">登録のトラブルシューティング イベント</span><span class="sxs-lookup"><span data-stu-id="4361f-130">Enrollment troubleshooting event</span></span>](intune_troubleshooting_enrollmenttroubleshootingevent.md)
- [<span data-ttu-id="4361f-131">ローカライズ済み通知メッセージ</span><span class="sxs-lookup"><span data-stu-id="4361f-131">Localized notification message</span></span>](intune_notification_localizednotificationmessage.md)
- [<span data-ttu-id="4361f-132">デバイスの検索アクションの結果</span><span class="sxs-lookup"><span data-stu-id="4361f-132">Locate device action result</span></span>](intune_devices_locatedeviceactionresult.md)
- [<span data-ttu-id="4361f-133">管理対象デバイスの概要</span><span class="sxs-lookup"><span data-stu-id="4361f-133">Managed device overview</span></span>](intune_devices_manageddeviceoverview.md)
- [<span data-ttu-id="4361f-134">管理対象デバイス</span><span class="sxs-lookup"><span data-stu-id="4361f-134">Managed device</span></span>](intune_devices_manageddevice.md)
- [<span data-ttu-id="4361f-135">通知メッセージ テンプレート</span><span class="sxs-lookup"><span data-stu-id="4361f-135">Notification message template</span></span>](intune_notification_notificationmessagetemplate.md)
- [<span data-ttu-id="4361f-136">リモート アシスタンス パートナー</span><span class="sxs-lookup"><span data-stu-id="4361f-136">Remote assistance partner</span></span>](intune_remoteassistance_remoteassistancepartner.md)
- [<span data-ttu-id="4361f-137">リモート ロック アクションの結果</span><span class="sxs-lookup"><span data-stu-id="4361f-137">Remote lock action result</span></span>](intune_devices_remotelockactionresult.md)
- [<span data-ttu-id="4361f-138">パスコードのリセット アクションの結果</span><span class="sxs-lookup"><span data-stu-id="4361f-138">Reset passcode action result</span></span>](intune_devices_resetpasscodeactionresult.md)
- [<span data-ttu-id="4361f-139">Windows のデバイス アカウントのアクション パラメーターの更新</span><span class="sxs-lookup"><span data-stu-id="4361f-139">Update windows device account action parameter</span></span>](intune_devices_updatewindowsdeviceaccountactionparameter.md)
- [<span data-ttu-id="4361f-140">ユーザー</span><span class="sxs-lookup"><span data-stu-id="4361f-140">User</span></span>](intune_devices_user.md)
- [<span data-ttu-id="4361f-141">ユーザー</span><span class="sxs-lookup"><span data-stu-id="4361f-141">User</span></span>](intune_troubleshooting_user.md)
- [<span data-ttu-id="4361f-142">Windows Defender のスキャン アクションの結果</span><span class="sxs-lookup"><span data-stu-id="4361f-142">Windows defender scan action result</span></span>](intune_devices_windowsdefenderscanactionresult.md)
- [<span data-ttu-id="4361f-143">Windows のデバイス アカウント</span><span class="sxs-lookup"><span data-stu-id="4361f-143">Windows device account</span></span>](intune_devices_windowsdeviceaccount.md)
- [<span data-ttu-id="4361f-144">Windows のデバイス AD アカウント</span><span class="sxs-lookup"><span data-stu-id="4361f-144">Windows device AD account</span></span>](intune_devices_windowsdeviceadaccount.md)
- [<span data-ttu-id="4361f-145">Windows のデバイス Azure AD アカウント</span><span class="sxs-lookup"><span data-stu-id="4361f-145">Windows device Azure AD account</span></span>](intune_devices_windowsdeviceazureadaccount.md)