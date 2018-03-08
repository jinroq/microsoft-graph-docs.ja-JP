# <a name="ebookinstallsummary-resource-type"></a><span data-ttu-id="b1411-101">eBookInstallSummary リソース タイプ</span><span class="sxs-lookup"><span data-stu-id="b1411-101">eBookInstallSummary resource type</span></span>

> <span data-ttu-id="b1411-102">**注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="b1411-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b1411-103">デバイスのブックのインストール要約のプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="b1411-103">Contains properties for the installation summary of a book for a device.</span></span>
## <a name="methods"></a><span data-ttu-id="b1411-104">メソッド</span><span class="sxs-lookup"><span data-stu-id="b1411-104">Methods</span></span>
|<span data-ttu-id="b1411-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="b1411-105">Method</span></span>|<span data-ttu-id="b1411-106">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="b1411-106">Return Type</span></span>|<span data-ttu-id="b1411-107">説明</span><span class="sxs-lookup"><span data-stu-id="b1411-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="b1411-108">Get eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="b1411-108">Get eBookInstallSummary</span></span>](../api/intune_books_ebookinstallsummary_get.md)|[<span data-ttu-id="b1411-109">eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="b1411-109">eBookInstallSummary</span></span>](../resources/intune_books_ebookinstallsummary.md)|<span data-ttu-id="b1411-110">[eBookInstallSummary](../resources/intune_books_ebookinstallsummary.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="b1411-110">Read properties and relationships of [plannerTaskDetails](../resources/intune_books_ebookinstallsummary.md) object.</span></span>|
|[<span data-ttu-id="b1411-111">Update eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="b1411-111">Update eBookInstallSummary</span></span>](../api/intune_books_ebookinstallsummary_update.md)|[<span data-ttu-id="b1411-112">eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="b1411-112">eBookInstallSummary</span></span>](../resources/intune_books_ebookinstallsummary.md)|<span data-ttu-id="b1411-113">[eBookInstallSummary](../resources/intune_books_ebookinstallsummary.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="b1411-113">Update the properties of a [calendar](../resources/intune_books_ebookinstallsummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="b1411-114">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b1411-114">Properties</span></span>
|<span data-ttu-id="b1411-115">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b1411-115">Property</span></span>|<span data-ttu-id="b1411-116">型</span><span class="sxs-lookup"><span data-stu-id="b1411-116">Type</span></span>|<span data-ttu-id="b1411-117">説明</span><span class="sxs-lookup"><span data-stu-id="b1411-117">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b1411-118">id</span><span class="sxs-lookup"><span data-stu-id="b1411-118">id</span></span>|<span data-ttu-id="b1411-119">String</span><span class="sxs-lookup"><span data-stu-id="b1411-119">String</span></span>|<span data-ttu-id="b1411-120">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="b1411-120">Name of the entity.</span></span>|
|<span data-ttu-id="b1411-121">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="b1411-121">installedDeviceCount</span></span>|<span data-ttu-id="b1411-122">Int32</span><span class="sxs-lookup"><span data-stu-id="b1411-122">Int32</span></span>|<span data-ttu-id="b1411-123">このブックが正常にインストールされたデバイスの数。</span><span class="sxs-lookup"><span data-stu-id="b1411-123">Number of Devices that have successfully installed this book.</span></span>|
|<span data-ttu-id="b1411-124">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="b1411-124">failedDeviceCount</span></span>|<span data-ttu-id="b1411-125">Int32</span><span class="sxs-lookup"><span data-stu-id="b1411-125">Int32</span></span>|<span data-ttu-id="b1411-126">このブックのインストールが失敗したデバイスの数。</span><span class="sxs-lookup"><span data-stu-id="b1411-126">Number of Devices that have failed to install this book.</span></span>|
|<span data-ttu-id="b1411-127">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="b1411-127">notInstalledDeviceCount</span></span>|<span data-ttu-id="b1411-128">Int32</span><span class="sxs-lookup"><span data-stu-id="b1411-128">Int32</span></span>|<span data-ttu-id="b1411-129">このブックがインストールされていないデバイスの数。</span><span class="sxs-lookup"><span data-stu-id="b1411-129">Number of Devices that does not have this book installed.</span></span>|
|<span data-ttu-id="b1411-130">installedUserCount</span><span class="sxs-lookup"><span data-stu-id="b1411-130">installedUserCount</span></span>|<span data-ttu-id="b1411-131">Int32</span><span class="sxs-lookup"><span data-stu-id="b1411-131">Int32</span></span>|<span data-ttu-id="b1411-132">このブックがすべて正常にインストールされたデバイスを所有しているユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="b1411-132">Number of Users whose devices have all succeeded to install this book.</span></span>|
|<span data-ttu-id="b1411-133">failedUserCount</span><span class="sxs-lookup"><span data-stu-id="b1411-133">failedUserCount</span></span>|<span data-ttu-id="b1411-134">Int32</span><span class="sxs-lookup"><span data-stu-id="b1411-134">Int32</span></span>|<span data-ttu-id="b1411-135">このブックのインストールが失敗したデバイスを 1 台以上所有しているユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="b1411-135">Number of Users that have 1 or more device that failed to install this book.</span></span>|
|<span data-ttu-id="b1411-136">notInstalledUserCount</span><span class="sxs-lookup"><span data-stu-id="b1411-136">notInstalledUserCount</span></span>|<span data-ttu-id="b1411-137">Int32</span><span class="sxs-lookup"><span data-stu-id="b1411-137">Int32</span></span>|<span data-ttu-id="b1411-138">このブックをインストールしていないユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="b1411-138">Number of Users that did not install this book.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b1411-139">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="b1411-139">Relationships</span></span>
<span data-ttu-id="b1411-140">なし</span><span class="sxs-lookup"><span data-stu-id="b1411-140">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="b1411-141">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b1411-141">JSON Representation</span></span>
<span data-ttu-id="b1411-142">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="b1411-142">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.eBookInstallSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.eBookInstallSummary",
  "id": "String (identifier)",
  "installedDeviceCount": 1024,
  "failedDeviceCount": 1024,
  "notInstalledDeviceCount": 1024,
  "installedUserCount": 1024,
  "failedUserCount": 1024,
  "notInstalledUserCount": 1024
}
```


