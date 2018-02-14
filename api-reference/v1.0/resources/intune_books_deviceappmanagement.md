# <a name="deviceappmanagement-resource-type"></a><span data-ttu-id="9f3e0-101">deviceAppManagement リソースの種類</span><span class="sxs-lookup"><span data-stu-id="9f3e0-101">deviceAppManagement resource type</span></span>

> <span data-ttu-id="9f3e0-102">**注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="9f3e0-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9f3e0-103">すべてのデバイス アプリの管理機能のコンテナーとして機能する単一のエンティティです。</span><span class="sxs-lookup"><span data-stu-id="9f3e0-103">Singleton entity that acts as a container for all device app management functionality.</span></span>
## <a name="methods"></a><span data-ttu-id="9f3e0-104">メソッド</span><span class="sxs-lookup"><span data-stu-id="9f3e0-104">Methods</span></span>
|<span data-ttu-id="9f3e0-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="9f3e0-105">Method</span></span>|<span data-ttu-id="9f3e0-106">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="9f3e0-106">Return Type</span></span>|<span data-ttu-id="9f3e0-107">説明</span><span class="sxs-lookup"><span data-stu-id="9f3e0-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="9f3e0-108">Get deviceAppManagement</span><span class="sxs-lookup"><span data-stu-id="9f3e0-108">Get deviceAppManagement</span></span>](../api/intune_books_deviceappmanagement_get.md)|[<span data-ttu-id="9f3e0-109">deviceAppManagement</span><span class="sxs-lookup"><span data-stu-id="9f3e0-109">deviceAppManagement</span></span>](../resources/intune_books_deviceappmanagement.md)|<span data-ttu-id="9f3e0-110">[deviceAppManagement](../resources/intune_books_deviceappmanagement.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="9f3e0-110">Read properties and relationships of [plannerTaskDetails](../resources/intune_books_deviceappmanagement.md) object.</span></span>|
|[<span data-ttu-id="9f3e0-111">Update deviceAppManagement</span><span class="sxs-lookup"><span data-stu-id="9f3e0-111">Update deviceAppManagement</span></span>](../api/intune_books_deviceappmanagement_update.md)|[<span data-ttu-id="9f3e0-112">deviceAppManagement</span><span class="sxs-lookup"><span data-stu-id="9f3e0-112">deviceAppManagement</span></span>](../resources/intune_books_deviceappmanagement.md)|<span data-ttu-id="9f3e0-113">[deviceAppManagement](../resources/intune_books_deviceappmanagement.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="9f3e0-113">Update the properties of a [calendar](../resources/intune_books_deviceappmanagement.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="9f3e0-114">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9f3e0-114">Properties</span></span>
|<span data-ttu-id="9f3e0-115">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9f3e0-115">Property</span></span>|<span data-ttu-id="9f3e0-116">型</span><span class="sxs-lookup"><span data-stu-id="9f3e0-116">Type</span></span>|<span data-ttu-id="9f3e0-117">説明</span><span class="sxs-lookup"><span data-stu-id="9f3e0-117">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9f3e0-118">id</span><span class="sxs-lookup"><span data-stu-id="9f3e0-118">id</span></span>|<span data-ttu-id="9f3e0-119">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="9f3e0-119">String</span></span>|<span data-ttu-id="9f3e0-120">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="9f3e0-120">Name of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9f3e0-121">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="9f3e0-121">Relationships</span></span>
|<span data-ttu-id="9f3e0-122">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="9f3e0-122">Relationship</span></span>|<span data-ttu-id="9f3e0-123">型</span><span class="sxs-lookup"><span data-stu-id="9f3e0-123">Type</span></span>|<span data-ttu-id="9f3e0-124">説明</span><span class="sxs-lookup"><span data-stu-id="9f3e0-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9f3e0-125">managedEBooks</span><span class="sxs-lookup"><span data-stu-id="9f3e0-125">managedEBooks</span></span>|<span data-ttu-id="9f3e0-126">[managedEBook](../resources/intune_books_managedebook.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="9f3e0-126">[managedEBook](../resources/intune_books_managedebook.md) collection</span></span>|<span data-ttu-id="9f3e0-127">管理対象の電子ブック。</span><span class="sxs-lookup"><span data-stu-id="9f3e0-127">The Managed eBook.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9f3e0-128">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="9f3e0-128">JSON Representation</span></span>
<span data-ttu-id="9f3e0-129">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="9f3e0-129">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceAppManagement"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceAppManagement",
  "id": "String (identifier)"
}
```



