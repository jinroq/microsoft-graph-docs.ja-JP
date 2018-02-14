# <a name="windowsinformationprotectiondatarecoverycertificate-resource-type"></a><span data-ttu-id="c9911-101">windowsInformationProtectionDataRecoveryCertificate リソースの種類</span><span class="sxs-lookup"><span data-stu-id="c9911-101">windowsInformationProtectionDataRecoveryCertificate resource type</span></span>

> <span data-ttu-id="c9911-102">**注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="c9911-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c9911-103">Windows 情報保護の DataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="c9911-103">Windows Information Protection DataRecoveryCertificate</span></span>
## <a name="properties"></a><span data-ttu-id="c9911-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c9911-104">Properties</span></span>
|<span data-ttu-id="c9911-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c9911-105">Property</span></span>|<span data-ttu-id="c9911-106">型</span><span class="sxs-lookup"><span data-stu-id="c9911-106">Type</span></span>|<span data-ttu-id="c9911-107">説明</span><span class="sxs-lookup"><span data-stu-id="c9911-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c9911-108">subjectName</span><span class="sxs-lookup"><span data-stu-id="c9911-108">subjectName</span></span>|<span data-ttu-id="c9911-109">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="c9911-109">String</span></span>|<span data-ttu-id="c9911-110">データ回復証明書のサブジェクト名</span><span class="sxs-lookup"><span data-stu-id="c9911-110">Data recovery Certificate subject name</span></span>|
|<span data-ttu-id="c9911-111">description</span><span class="sxs-lookup"><span data-stu-id="c9911-111">description</span></span>|<span data-ttu-id="c9911-112">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="c9911-112">String</span></span>|<span data-ttu-id="c9911-113">データ回復証明書の説明</span><span class="sxs-lookup"><span data-stu-id="c9911-113">Data recovery Certificate description</span></span>|
|<span data-ttu-id="c9911-114">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="c9911-114">expirationDateTime</span></span>|<span data-ttu-id="c9911-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c9911-115">DateTimeOffset</span></span>|<span data-ttu-id="c9911-116">データ回復証明書の有効期限日時</span><span class="sxs-lookup"><span data-stu-id="c9911-116">Data recovery Certificate expiration datetime</span></span>|
|<span data-ttu-id="c9911-117">certificate</span><span class="sxs-lookup"><span data-stu-id="c9911-117">ACS, certificate</span></span>|<span data-ttu-id="c9911-118">バイナリ型 (Binary)</span><span class="sxs-lookup"><span data-stu-id="c9911-118">Binary</span></span>|<span data-ttu-id="c9911-119">データ回復証明書</span><span class="sxs-lookup"><span data-stu-id="c9911-119">Data recovery Certificate</span></span>|

## <a name="relationships"></a><span data-ttu-id="c9911-120">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="c9911-120">Relationships</span></span>
<span data-ttu-id="c9911-121">なし</span><span class="sxs-lookup"><span data-stu-id="c9911-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="c9911-122">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c9911-122">JSON Representation</span></span>
<span data-ttu-id="c9911-123">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="c9911-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsInformationProtectionDataRecoveryCertificate"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionDataRecoveryCertificate",
  "subjectName": "String",
  "description": "String",
  "expirationDateTime": "String (timestamp)",
  "certificate": "binary"
}
```



