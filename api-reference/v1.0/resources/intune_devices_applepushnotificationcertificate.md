# <a name="applepushnotificationcertificate-resource-type"></a><span data-ttu-id="df018-101">applePushNotificationCertificate リソースの種類</span><span class="sxs-lookup"><span data-stu-id="df018-101">applePushNotificationCertificate resource type</span></span>

> <span data-ttu-id="df018-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="df018-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="df018-103">Apple プッシュ通知証明書。</span><span class="sxs-lookup"><span data-stu-id="df018-103">Apple push notification certificate.</span></span>
## <a name="methods"></a><span data-ttu-id="df018-104">メソッド</span><span class="sxs-lookup"><span data-stu-id="df018-104">Methods</span></span>
|<span data-ttu-id="df018-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="df018-105">Method</span></span>|<span data-ttu-id="df018-106">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="df018-106">Return Type</span></span>|<span data-ttu-id="df018-107">説明</span><span class="sxs-lookup"><span data-stu-id="df018-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="df018-108">Get applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="df018-108">Get applePushNotificationCertificate</span></span>](../api/intune_devices_applepushnotificationcertificate_get.md)|[<span data-ttu-id="df018-109">applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="df018-109">applePushNotificationCertificate</span></span>](../resources/intune_devices_applepushnotificationcertificate.md)|<span data-ttu-id="df018-110">[applePushNotificationCertificate](../resources/intune_devices_applepushnotificationcertificate.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="df018-110">Read properties and relationships of the [applePushNotificationCertificate](../resources/intune_devices_applepushnotificationcertificate.md) object.</span></span>|
|[<span data-ttu-id="df018-111">Update applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="df018-111">Update applePushNotificationCertificate</span></span>](../api/intune_devices_applepushnotificationcertificate_update.md)|[<span data-ttu-id="df018-112">applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="df018-112">applePushNotificationCertificate</span></span>](../resources/intune_devices_applepushnotificationcertificate.md)|<span data-ttu-id="df018-113">[applePushNotificationCertificate](../resources/intune_devices_applepushnotificationcertificate.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="df018-113">Update the properties of a [applePushNotificationCertificate](../resources/intune_devices_applepushnotificationcertificate.md) object.</span></span>|
|[<span data-ttu-id="df018-114">downloadApplePushNotificationCertificateSigningRequest 関数</span><span class="sxs-lookup"><span data-stu-id="df018-114">downloadApplePushNotificationCertificateSigningRequest function</span></span>](../api/intune_devices_applepushnotificationcertificate_downloadapplepushnotificationcertificatesigningrequest.md)|<span data-ttu-id="df018-115">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="df018-115">String</span></span>|<span data-ttu-id="df018-116">Apple プッシュ通知の証明書署名要求をダウンロードします</span><span class="sxs-lookup"><span data-stu-id="df018-116">Download Apple push notification certificate signing request</span></span>|

## <a name="properties"></a><span data-ttu-id="df018-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="df018-117">Properties</span></span>
|<span data-ttu-id="df018-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="df018-118">Property</span></span>|<span data-ttu-id="df018-119">型</span><span class="sxs-lookup"><span data-stu-id="df018-119">Type</span></span>|<span data-ttu-id="df018-120">説明</span><span class="sxs-lookup"><span data-stu-id="df018-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="df018-121">id</span><span class="sxs-lookup"><span data-stu-id="df018-121">id</span></span>|<span data-ttu-id="df018-122">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="df018-122">String</span></span>|<span data-ttu-id="df018-123">証明書の一意識別子</span><span class="sxs-lookup"><span data-stu-id="df018-123">Unique Identifier for the certificate</span></span>|
|<span data-ttu-id="df018-124">appleIdentifier</span><span class="sxs-lookup"><span data-stu-id="df018-124">appleIdentifier</span></span>|<span data-ttu-id="df018-125">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="df018-125">String</span></span>|<span data-ttu-id="df018-126">MDM プッシュ証明書の作成に使用するアカウントの Apple ID。</span><span class="sxs-lookup"><span data-stu-id="df018-126">Apple Id of the account used to create the MDM push certificate.</span></span>|
|<span data-ttu-id="df018-127">topicIdentifier</span><span class="sxs-lookup"><span data-stu-id="df018-127">topicIdentifier</span></span>|<span data-ttu-id="df018-128">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="df018-128">String</span></span>|<span data-ttu-id="df018-129">トピック ID。</span><span class="sxs-lookup"><span data-stu-id="df018-129">Topic Id.</span></span>|
|<span data-ttu-id="df018-130">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="df018-130">lastModifiedDateTime</span></span>|<span data-ttu-id="df018-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="df018-131">DateTimeOffset</span></span>|<span data-ttu-id="df018-132">Apple プッシュ通知証明書の最終変更日時。</span><span class="sxs-lookup"><span data-stu-id="df018-132">Last modified date and time for Apple push notification certificate.</span></span>|
|<span data-ttu-id="df018-133">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="df018-133">expirationDateTime</span></span>|<span data-ttu-id="df018-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="df018-134">DateTimeOffset</span></span>|<span data-ttu-id="df018-135">Apple プッシュ通知証明書の有効期限。</span><span class="sxs-lookup"><span data-stu-id="df018-135">The expiration date and time for Apple push notification certificate.</span></span>|
|<span data-ttu-id="df018-136">certificate</span><span class="sxs-lookup"><span data-stu-id="df018-136">certificate</span></span>|<span data-ttu-id="df018-137">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="df018-137">String</span></span>|<span data-ttu-id="df018-138">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="df018-138">Not yet documented</span></span>|

## <a name="relationships"></a><span data-ttu-id="df018-139">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="df018-139">Relationships</span></span>
<span data-ttu-id="df018-140">なし</span><span class="sxs-lookup"><span data-stu-id="df018-140">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="df018-141">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="df018-141">JSON Representation</span></span>
<span data-ttu-id="df018-142">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="df018-142">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.applePushNotificationCertificate"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.applePushNotificationCertificate",
  "id": "String (identifier)",
  "appleIdentifier": "String",
  "topicIdentifier": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "expirationDateTime": "String (timestamp)",
  "certificate": "String"
}
```



