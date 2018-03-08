# <a name="iosnotificationsettings-resource-type"></a><span data-ttu-id="5efcf-101">iosNotificationSettings リソース タイプ</span><span class="sxs-lookup"><span data-stu-id="5efcf-101">iosNotificationSettings resource type</span></span>

> <span data-ttu-id="5efcf-102">**注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="5efcf-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5efcf-103">通知設定を記述するアイテムです。</span><span class="sxs-lookup"><span data-stu-id="5efcf-103">An item describing notification setting.</span></span>
## <a name="properties"></a><span data-ttu-id="5efcf-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5efcf-104">Properties</span></span>
|<span data-ttu-id="5efcf-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5efcf-105">Property</span></span>|<span data-ttu-id="5efcf-106">型</span><span class="sxs-lookup"><span data-stu-id="5efcf-106">Type</span></span>|<span data-ttu-id="5efcf-107">説明</span><span class="sxs-lookup"><span data-stu-id="5efcf-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5efcf-108">bundleID</span><span class="sxs-lookup"><span data-stu-id="5efcf-108">bundleID</span></span>|<span data-ttu-id="5efcf-109">String</span><span class="sxs-lookup"><span data-stu-id="5efcf-109">String</span></span>|<span data-ttu-id="5efcf-110">これらの通知設定を適用するアプリのバンドル ID。</span><span class="sxs-lookup"><span data-stu-id="5efcf-110">Bundle id of app to which to apply these notification settings.</span></span>|
|<span data-ttu-id="5efcf-111">appName</span><span class="sxs-lookup"><span data-stu-id="5efcf-111">appname</span></span>|<span data-ttu-id="5efcf-112">String</span><span class="sxs-lookup"><span data-stu-id="5efcf-112">String</span></span>|<span data-ttu-id="5efcf-113">bundleID に関連するアプリケーション名。</span><span class="sxs-lookup"><span data-stu-id="5efcf-113">Application name to be associated with the bundleID.</span></span>|
|<span data-ttu-id="5efcf-114">publisher</span><span class="sxs-lookup"><span data-stu-id="5efcf-114">Publisher</span></span>|<span data-ttu-id="5efcf-115">String</span><span class="sxs-lookup"><span data-stu-id="5efcf-115">String</span></span>|<span data-ttu-id="5efcf-116">bundleID に関連するパブリッシャー。</span><span class="sxs-lookup"><span data-stu-id="5efcf-116">Publisher to be associated with the bundleID.</span></span>|
|<span data-ttu-id="5efcf-117">enabled</span><span class="sxs-lookup"><span data-stu-id="5efcf-117">enabled</span></span>|<span data-ttu-id="5efcf-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="5efcf-118">Boolean</span></span>|<span data-ttu-id="5efcf-119">通知がこのアプリで許可されているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="5efcf-119">Indicates whether notifications are allowed for this app.</span></span>|
|<span data-ttu-id="5efcf-120">showInNotificationCenter</span><span class="sxs-lookup"><span data-stu-id="5efcf-120">showInNotificationCenter</span></span>|<span data-ttu-id="5efcf-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="5efcf-121">Boolean</span></span>|<span data-ttu-id="5efcf-122">通知センターに通知を表示できるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="5efcf-122">Indicates whether notifications can be shown in notification center.</span></span>|
|<span data-ttu-id="5efcf-123">showOnLockScreen</span><span class="sxs-lookup"><span data-stu-id="5efcf-123">showOnLockScreen</span></span>|<span data-ttu-id="5efcf-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="5efcf-124">Boolean</span></span>|<span data-ttu-id="5efcf-125">ロック画面に通知を表示できるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="5efcf-125">Indicates whether notifications can be shown on the lock screen.</span></span>|
|<span data-ttu-id="5efcf-126">alertType</span><span class="sxs-lookup"><span data-stu-id="5efcf-126">alertType</span></span>|<span data-ttu-id="5efcf-127">String</span><span class="sxs-lookup"><span data-stu-id="5efcf-127">String</span></span>|<span data-ttu-id="5efcf-128">このアプリの通知用の警告の種類を示します。</span><span class="sxs-lookup"><span data-stu-id="5efcf-128">Indicates the type of alert for notifications for this app.</span></span> <span data-ttu-id="5efcf-129">可能な値は、`deviceDefault`、`banner`、`modal`、`none` です。</span><span class="sxs-lookup"><span data-stu-id="5efcf-129">Possible values are: `deviceDefault`, `banner`, `modal`, `none`.</span></span>|
|<span data-ttu-id="5efcf-130">badgesEnabled</span><span class="sxs-lookup"><span data-stu-id="5efcf-130">badgesEnabled</span></span>|<span data-ttu-id="5efcf-131">Boolean</span><span class="sxs-lookup"><span data-stu-id="5efcf-131">Boolean</span></span>|<span data-ttu-id="5efcf-132">バッジがこのアプリで許可されているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="5efcf-132">Indicates whether badges are allowed for this app.</span></span>|
|<span data-ttu-id="5efcf-133">soundsEnabled</span><span class="sxs-lookup"><span data-stu-id="5efcf-133">soundsEnabled</span></span>|<span data-ttu-id="5efcf-134">Boolean</span><span class="sxs-lookup"><span data-stu-id="5efcf-134">Boolean</span></span>|<span data-ttu-id="5efcf-135">サウンドがこのアプリで許可されているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="5efcf-135">Indicates whether sounds are allowed for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5efcf-136">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="5efcf-136">Relationships</span></span>
<span data-ttu-id="5efcf-137">なし</span><span class="sxs-lookup"><span data-stu-id="5efcf-137">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="5efcf-138">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="5efcf-138">JSON Representation</span></span>
<span data-ttu-id="5efcf-139">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="5efcf-139">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.iosNotificationSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosNotificationSettings",
  "bundleID": "String",
  "appName": "String",
  "publisher": "String",
  "enabled": true,
  "showInNotificationCenter": true,
  "showOnLockScreen": true,
  "alertType": "String",
  "badgesEnabled": true,
  "soundsEnabled": true
}
```


