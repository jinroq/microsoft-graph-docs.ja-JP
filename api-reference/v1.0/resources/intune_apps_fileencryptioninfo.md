# <a name="fileencryptioninfo-resource-type"></a><span data-ttu-id="4a82f-101">fileEncryptionInfo リソースの種類</span><span class="sxs-lookup"><span data-stu-id="4a82f-101">fileEncryptionInfo resource type</span></span>

> <span data-ttu-id="4a82f-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="4a82f-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4a82f-103">ビジネス アプリの行のコンテンツ バージョンのファイル暗号化情報のプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="4a82f-103">Contains properties for file encryption information for the content version of a line of business app.</span></span>
## <a name="properties"></a><span data-ttu-id="4a82f-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4a82f-104">Properties</span></span>
|<span data-ttu-id="4a82f-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4a82f-105">Property</span></span>|<span data-ttu-id="4a82f-106">タイプ</span><span class="sxs-lookup"><span data-stu-id="4a82f-106">Type</span></span>|<span data-ttu-id="4a82f-107">説明</span><span class="sxs-lookup"><span data-stu-id="4a82f-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4a82f-108">encryptionKey</span><span class="sxs-lookup"><span data-stu-id="4a82f-108">encryptionKey</span></span>|<span data-ttu-id="4a82f-109">Binary</span><span class="sxs-lookup"><span data-stu-id="4a82f-109">Binary</span></span>|<span data-ttu-id="4a82f-110">ファイルのコンテンツを暗号化するために使用するキーです。</span><span class="sxs-lookup"><span data-stu-id="4a82f-110">The key used to encrypt the file content.</span></span>|
|<span data-ttu-id="4a82f-111">initializationVector</span><span class="sxs-lookup"><span data-stu-id="4a82f-111">initializationVector</span></span>|<span data-ttu-id="4a82f-112">Binary</span><span class="sxs-lookup"><span data-stu-id="4a82f-112">Binary</span></span>|<span data-ttu-id="4a82f-113">暗号化アルゴリズムに使用される初期化ベクトルです。</span><span class="sxs-lookup"><span data-stu-id="4a82f-113">The initialization vector used for the encryption algorithm.</span></span>|
|<span data-ttu-id="4a82f-114">Mac</span><span class="sxs-lookup"><span data-stu-id="4a82f-114">mac</span></span>|<span data-ttu-id="4a82f-115">Binary</span><span class="sxs-lookup"><span data-stu-id="4a82f-115">Binary</span></span>|<span data-ttu-id="4a82f-116">暗号化されたファイル コンテンツのハッシュ + IV (コンテンツ ハッシュ) です。</span><span class="sxs-lookup"><span data-stu-id="4a82f-116">The hash of the encrypted file content + IV (content hash).</span></span>|
|<span data-ttu-id="4a82f-117">macKey</span><span class="sxs-lookup"><span data-stu-id="4a82f-117">macKey</span></span>|<span data-ttu-id="4a82f-118">Binary</span><span class="sxs-lookup"><span data-stu-id="4a82f-118">Binary</span></span>|<span data-ttu-id="4a82f-119">Mac を取得するために使用するキーです。</span><span class="sxs-lookup"><span data-stu-id="4a82f-119">The key used to get mac.</span></span>|
|<span data-ttu-id="4a82f-120">profileIdentifier</span><span class="sxs-lookup"><span data-stu-id="4a82f-120">profileIdentifier</span></span>|<span data-ttu-id="4a82f-121">String</span><span class="sxs-lookup"><span data-stu-id="4a82f-121">String</span></span>|<span data-ttu-id="4a82f-122">プロファイルの識別子です。</span><span class="sxs-lookup"><span data-stu-id="4a82f-122">The the profile identifier.</span></span>|
|<span data-ttu-id="4a82f-123">fileDigest</span><span class="sxs-lookup"><span data-stu-id="4a82f-123">fileDigest</span></span>|<span data-ttu-id="4a82f-124">Binary</span><span class="sxs-lookup"><span data-stu-id="4a82f-124">Binary</span></span>|<span data-ttu-id="4a82f-125">暗号化される前のファイル ダイジェストです。</span><span class="sxs-lookup"><span data-stu-id="4a82f-125">The file digest prior to encryption.</span></span>|
|<span data-ttu-id="4a82f-126">fileDigestAlgorithm</span><span class="sxs-lookup"><span data-stu-id="4a82f-126">fileDigestAlgorithm</span></span>|<span data-ttu-id="4a82f-127">String</span><span class="sxs-lookup"><span data-stu-id="4a82f-127">String</span></span>|<span data-ttu-id="4a82f-128">ファイル ダイジェストのアルゴリズムです。</span><span class="sxs-lookup"><span data-stu-id="4a82f-128">The file digest algorithm.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4a82f-129">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="4a82f-129">Relationships</span></span>
<span data-ttu-id="4a82f-130">なし</span><span class="sxs-lookup"><span data-stu-id="4a82f-130">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="4a82f-131">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="4a82f-131">JSON Representation</span></span>
<span data-ttu-id="4a82f-132">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="4a82f-132">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.fileEncryptionInfo"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.fileEncryptionInfo",
  "encryptionKey": "binary",
  "initializationVector": "binary",
  "mac": "binary",
  "macKey": "binary",
  "profileIdentifier": "String",
  "fileDigest": "binary",
  "fileDigestAlgorithm": "String"
}
```



