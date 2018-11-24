# <a name="bitlockerremovabledrivepolicy-resource-type"></a><span data-ttu-id="e6b77-101">bitLockerRemovableDrivePolicy リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e6b77-101">bitLockerRemovableDrivePolicy resource type</span></span>

> <span data-ttu-id="e6b77-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="e6b77-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e6b77-103">BitLocker リムーバブル ドライブ ポリシー。</span><span class="sxs-lookup"><span data-stu-id="e6b77-103">BitLocker Removable Drive Policies.</span></span>
## <a name="properties"></a><span data-ttu-id="e6b77-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e6b77-104">Properties</span></span>
|<span data-ttu-id="e6b77-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e6b77-105">Property</span></span>|<span data-ttu-id="e6b77-106">型</span><span class="sxs-lookup"><span data-stu-id="e6b77-106">Type</span></span>|<span data-ttu-id="e6b77-107">説明</span><span class="sxs-lookup"><span data-stu-id="e6b77-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e6b77-108">encryptionMethod</span><span class="sxs-lookup"><span data-stu-id="e6b77-108">encryptionMethod</span></span>|[<span data-ttu-id="e6b77-109">bitLockerEncryptionMethod</span><span class="sxs-lookup"><span data-stu-id="e6b77-109">bitLockerEncryptionMethod</span></span>](../resources/intune_deviceconfig_bitlockerencryptionmethod.md)|<span data-ttu-id="e6b77-110">リムーバブル ドライブの暗号化方法を選択します。</span><span class="sxs-lookup"><span data-stu-id="e6b77-110">Select the encryption method for removable  drives.</span></span> <span data-ttu-id="e6b77-111">可能な値は、`aesCbc128`、`aesCbc256`、`xtsAes128`、`xtsAes256` です。</span><span class="sxs-lookup"><span data-stu-id="e6b77-111">Possible values are: `aesCbc128`, `aesCbc256`, `xtsAes128`, `xtsAes256`.</span></span>|
|<span data-ttu-id="e6b77-112">requireEncryptionForWriteAccess</span><span class="sxs-lookup"><span data-stu-id="e6b77-112">requireEncryptionForWriteAccess</span></span>|<span data-ttu-id="e6b77-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="e6b77-113">Boolean</span></span>|<span data-ttu-id="e6b77-114">別の組織で構成されたデバイスへの書き込みアクセスをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="e6b77-114">Indicates whether to block write access to devices configured in another organization.</span></span>  <span data-ttu-id="e6b77-115">RequireEncryptionForWriteAccess が false の場合、この値は影響を与えません。</span><span class="sxs-lookup"><span data-stu-id="e6b77-115">If requireEncryptionForWriteAccess is false, this value does not affect.</span></span>|
|<span data-ttu-id="e6b77-116">blockCrossOrganizationWriteAccess</span><span class="sxs-lookup"><span data-stu-id="e6b77-116">blockCrossOrganizationWriteAccess</span></span>|<span data-ttu-id="e6b77-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="e6b77-117">Boolean</span></span>|<span data-ttu-id="e6b77-118">このポリシー設定は、コンピューター上でリムーバブル データ ドライブを書き込み可能にする際に、BitLocker 保護が必要かどうかを決定します。</span><span class="sxs-lookup"><span data-stu-id="e6b77-118">This policy setting determines whether BitLocker protection is required for removable data drives to be writable on a computer.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e6b77-119">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="e6b77-119">Relationships</span></span>
<span data-ttu-id="e6b77-120">なし</span><span class="sxs-lookup"><span data-stu-id="e6b77-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="e6b77-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e6b77-121">JSON Representation</span></span>
<span data-ttu-id="e6b77-122">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="e6b77-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
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



