# <a name="bitlockerremovabledrivepolicy-resource-type"></a><span data-ttu-id="6dcad-101">bitLockerRemovableDrivePolicy リソースの種類</span><span class="sxs-lookup"><span data-stu-id="6dcad-101">bitLockerRemovableDrivePolicy resource type</span></span>

> <span data-ttu-id="6dcad-102">**注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="6dcad-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6dcad-103">BitLocker リムーバブル ドライブ ポリシー。</span><span class="sxs-lookup"><span data-stu-id="6dcad-103">BitLocker Removable Drive Policies.</span></span>
## <a name="properties"></a><span data-ttu-id="6dcad-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6dcad-104">Properties</span></span>
|<span data-ttu-id="6dcad-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6dcad-105">Property</span></span>|<span data-ttu-id="6dcad-106">型</span><span class="sxs-lookup"><span data-stu-id="6dcad-106">Type</span></span>|<span data-ttu-id="6dcad-107">説明</span><span class="sxs-lookup"><span data-stu-id="6dcad-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6dcad-108">encryptionMethod</span><span class="sxs-lookup"><span data-stu-id="6dcad-108">encryptionMethod</span></span>|<span data-ttu-id="6dcad-109">String</span><span class="sxs-lookup"><span data-stu-id="6dcad-109">String</span></span>|<span data-ttu-id="6dcad-110">リムーバブル ドライブの暗号化方法を選択します。</span><span class="sxs-lookup"><span data-stu-id="6dcad-110">Select the encryption method for removable  drives.</span></span> <span data-ttu-id="6dcad-111">可能な値は、`aesCbc128`、`aesCbc256`、`xtsAes128`、`xtsAes256` です。</span><span class="sxs-lookup"><span data-stu-id="6dcad-111">Possible values are: `aesCbc128`, `aesCbc256`, `xtsAes128`, `xtsAes256`.</span></span>|
|<span data-ttu-id="6dcad-112">requireEncryptionForWriteAccess</span><span class="sxs-lookup"><span data-stu-id="6dcad-112">requireEncryptionForWriteAccess</span></span>|<span data-ttu-id="6dcad-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="6dcad-113">Boolean</span></span>|<span data-ttu-id="6dcad-114">別の組織で構成されたデバイスへの書き込みアクセスをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6dcad-114">Indicates whether to block write access to devices configured in another organization.</span></span>  <span data-ttu-id="6dcad-115">RequireEncryptionForWriteAccess が false の場合、この値は影響を与えません。</span><span class="sxs-lookup"><span data-stu-id="6dcad-115">If requireEncryptionForWriteAccess is false, this value does not affect.</span></span>|
|<span data-ttu-id="6dcad-116">blockCrossOrganizationWriteAccess</span><span class="sxs-lookup"><span data-stu-id="6dcad-116">blockCrossOrganizationWriteAccess</span></span>|<span data-ttu-id="6dcad-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="6dcad-117">Boolean</span></span>|<span data-ttu-id="6dcad-118">このポリシー設定は、コンピューター上でリムーバブル データ ドライブを書き込み可能にする際に、BitLocker 保護が必要かどうかを決定します。</span><span class="sxs-lookup"><span data-stu-id="6dcad-118">This policy setting determines whether BitLocker protection is required for removable data drives to be writable on a computer.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6dcad-119">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="6dcad-119">Relationships</span></span>
<span data-ttu-id="6dcad-120">なし</span><span class="sxs-lookup"><span data-stu-id="6dcad-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="6dcad-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="6dcad-121">JSON Representation</span></span>
<span data-ttu-id="6dcad-122">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="6dcad-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.bitLockerRemovableDrivePolicy"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.bitLockerRemovableDrivePolicy",
  "encryptionMethod": "String",
  "requireEncryptionForWriteAccess": true,
  "blockCrossOrganizationWriteAccess": true
}
```



