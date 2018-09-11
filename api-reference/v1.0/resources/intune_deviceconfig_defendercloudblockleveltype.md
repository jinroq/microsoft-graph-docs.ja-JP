# <a name="defendercloudblockleveltype-enum-type"></a><span data-ttu-id="ff4bf-101">defenderCloudBlockLevelType 列挙型</span><span class="sxs-lookup"><span data-stu-id="ff4bf-101">defenderCloudBlockLevelType enum type</span></span>

> <span data-ttu-id="ff4bf-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="ff4bf-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ff4bf-103">クラウド ブロック レベルの使用可能な値</span><span class="sxs-lookup"><span data-stu-id="ff4bf-103">Possible values of Cloud Block Level</span></span>
## <a name="members"></a><span data-ttu-id="ff4bf-104">メンバー</span><span class="sxs-lookup"><span data-stu-id="ff4bf-104">Members</span></span>
|<span data-ttu-id="ff4bf-105">メンバー</span><span class="sxs-lookup"><span data-stu-id="ff4bf-105">Member</span></span>|<span data-ttu-id="ff4bf-106">値</span><span class="sxs-lookup"><span data-stu-id="ff4bf-106">Value</span></span>|<span data-ttu-id="ff4bf-107">説明</span><span class="sxs-lookup"><span data-stu-id="ff4bf-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ff4bf-108">notConfigured</span><span class="sxs-lookup"><span data-stu-id="ff4bf-108">notConfigured</span></span>|<span data-ttu-id="ff4bf-109">0</span><span class="sxs-lookup"><span data-stu-id="ff4bf-109">0%</span></span>|<span data-ttu-id="ff4bf-110">既定値、規定の Windows Defender アンチウイルス ソフトウェアのブロック レベルを使用、正規ファイルを検出するリスクを増大させることなく強力な検出性能を提供</span><span class="sxs-lookup"><span data-stu-id="ff4bf-110">Default value, uses the default Windows Defender Antivirus blocking level and provides strong detection without increasing the risk of detecting legitimate files</span></span>|
|<span data-ttu-id="ff4bf-111">high</span><span class="sxs-lookup"><span data-stu-id="ff4bf-111">High.</span></span>|<span data-ttu-id="ff4bf-112">1</span><span class="sxs-lookup"><span data-stu-id="ff4bf-112">-1</span></span>|<span data-ttu-id="ff4bf-113">"高" は強力な検出レベルを適用します。</span><span class="sxs-lookup"><span data-stu-id="ff4bf-113">High applies a strong level of detection.</span></span>|
|<span data-ttu-id="ff4bf-114">highPlus</span><span class="sxs-lookup"><span data-stu-id="ff4bf-114">highPlus</span></span>|<span data-ttu-id="ff4bf-115">2</span><span class="sxs-lookup"><span data-stu-id="ff4bf-115">-2</span></span>|<span data-ttu-id="ff4bf-116">"高 +" は、高レベルを使用し、追加の保護手段を適用します。</span><span class="sxs-lookup"><span data-stu-id="ff4bf-116">High + uses the High level and applies addition protection measures</span></span>|
|<span data-ttu-id="ff4bf-117">zeroTolerance</span><span class="sxs-lookup"><span data-stu-id="ff4bf-117">zeroTolerance</span></span>|<span data-ttu-id="ff4bf-118">3</span><span class="sxs-lookup"><span data-stu-id="ff4bf-118">"3"</span></span>|<span data-ttu-id="ff4bf-119">"ゼロ容認" は、すべての不明な実行ファイルをブロックします。</span><span class="sxs-lookup"><span data-stu-id="ff4bf-119">Zero tolerance blocks all unknown executables</span></span>|








