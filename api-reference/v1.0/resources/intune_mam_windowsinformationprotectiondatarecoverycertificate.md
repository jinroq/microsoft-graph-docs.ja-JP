# <a name="windowsinformationprotectiondatarecoverycertificate-resource-type"></a><span data-ttu-id="0a367-101">windowsInformationProtectionDataRecoveryCertificate リソースの種類</span><span class="sxs-lookup"><span data-stu-id="0a367-101">windowsInformationProtectionDataRecoveryCertificate resource type</span></span>

> <span data-ttu-id="0a367-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="0a367-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0a367-103">Windows 情報保護の DataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="0a367-103">Windows Information Protection DataRecoveryCertificate</span></span>
## <a name="properties"></a><span data-ttu-id="0a367-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0a367-104">Properties</span></span>
|<span data-ttu-id="0a367-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0a367-105">Property</span></span>|<span data-ttu-id="0a367-106">タイプ</span><span class="sxs-lookup"><span data-stu-id="0a367-106">Type</span></span>|<span data-ttu-id="0a367-107">説明</span><span class="sxs-lookup"><span data-stu-id="0a367-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0a367-108">subjectName</span><span class="sxs-lookup"><span data-stu-id="0a367-108">subjectName</span></span>|<span data-ttu-id="0a367-109">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="0a367-109">String</span></span>|<span data-ttu-id="0a367-110">データ回復証明書のサブジェクト名</span><span class="sxs-lookup"><span data-stu-id="0a367-110">Data recovery Certificate subject name</span></span>|
|<span data-ttu-id="0a367-111">説明</span><span class="sxs-lookup"><span data-stu-id="0a367-111">description</span></span>|<span data-ttu-id="0a367-112">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="0a367-112">String</span></span>|<span data-ttu-id="0a367-113">データ回復証明書の説明</span><span class="sxs-lookup"><span data-stu-id="0a367-113">Data recovery Certificate description</span></span>|
|<span data-ttu-id="0a367-114">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="0a367-114">expirationDateTime</span></span>|<span data-ttu-id="0a367-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0a367-115">DateTimeOffset</span></span>|<span data-ttu-id="0a367-116">データ回復証明書の有効期限日時</span><span class="sxs-lookup"><span data-stu-id="0a367-116">Data recovery Certificate expiration datetime</span></span>|
|<span data-ttu-id="0a367-117">証明書</span><span class="sxs-lookup"><span data-stu-id="0a367-117">certificate</span></span>|<span data-ttu-id="0a367-118">バイナリ型 (Binary)</span><span class="sxs-lookup"><span data-stu-id="0a367-118">Binary</span></span>|<span data-ttu-id="0a367-119">データ回復証明書</span><span class="sxs-lookup"><span data-stu-id="0a367-119">Data recovery Certificate</span></span>|

## <a name="relationships"></a><span data-ttu-id="0a367-120">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="0a367-120">Relationships</span></span>
<span data-ttu-id="0a367-121">なし</span><span class="sxs-lookup"><span data-stu-id="0a367-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="0a367-122">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="0a367-122">JSON Representation</span></span>
<span data-ttu-id="0a367-123">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="0a367-123">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsInformationProtectionDataRecoveryCertificate"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionDataRecoveryCertificate",
  "subjectName": "String",
  "description": "String",
  "expirationDateTime": "String (timestamp)",
  "certificate": "binary"
}
```



