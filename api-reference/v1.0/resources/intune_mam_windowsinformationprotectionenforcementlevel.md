# <a name="windowsinformationprotectionenforcementlevel-enum-type"></a><span data-ttu-id="0c787-101">windowsInformationProtectionEnforcementLevel 列挙型</span><span class="sxs-lookup"><span data-stu-id="0c787-101">windowsInformationProtectionEnforcementLevel enum type</span></span>

> <span data-ttu-id="0c787-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="0c787-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0c787-103">WIP保護を実施レベルに指定できる値</span><span class="sxs-lookup"><span data-stu-id="0c787-103">Possible values for WIP Protection enforcement levels</span></span>
## <a name="members"></a><span data-ttu-id="0c787-104">メンバー</span><span class="sxs-lookup"><span data-stu-id="0c787-104">Members</span></span>
|<span data-ttu-id="0c787-105">メンバー</span><span class="sxs-lookup"><span data-stu-id="0c787-105">Member</span></span>|<span data-ttu-id="0c787-106">値</span><span class="sxs-lookup"><span data-stu-id="0c787-106">Value</span></span>|<span data-ttu-id="0c787-107">説明</span><span class="sxs-lookup"><span data-stu-id="0c787-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0c787-108">noProtection</span><span class="sxs-lookup"><span data-stu-id="0c787-108">noProtection</span></span>|<span data-ttu-id="0c787-109">0</span><span class="sxs-lookup"><span data-stu-id="0c787-109">0%</span></span>|<span data-ttu-id="0c787-110">保護の実施なし</span><span class="sxs-lookup"><span data-stu-id="0c787-110">No protection enforcement</span></span>|
|<span data-ttu-id="0c787-111">encryptAndAuditOnly</span><span class="sxs-lookup"><span data-stu-id="0c787-111">encryptAndAuditOnly</span></span>|<span data-ttu-id="0c787-112">1</span><span class="sxs-lookup"><span data-stu-id="0c787-112">-1</span></span>|<span data-ttu-id="0c787-113">暗号化と監査のみ</span><span class="sxs-lookup"><span data-stu-id="0c787-113">Encrypt and Audit only</span></span>|
|<span data-ttu-id="0c787-114">encryptAuditAndPrompt</span><span class="sxs-lookup"><span data-stu-id="0c787-114">encryptAuditAndPrompt</span></span>|<span data-ttu-id="0c787-115">2</span><span class="sxs-lookup"><span data-stu-id="0c787-115">-2</span></span>|<span data-ttu-id="0c787-116">暗号化、監査、およびダイアログの表示</span><span class="sxs-lookup"><span data-stu-id="0c787-116">Encrypt, Audit and Prompt</span></span>|
|<span data-ttu-id="0c787-117">encryptAuditAndBlock</span><span class="sxs-lookup"><span data-stu-id="0c787-117">encryptAuditAndBlock</span></span>|<span data-ttu-id="0c787-118">3</span><span class="sxs-lookup"><span data-stu-id="0c787-118">"3"</span></span>|<span data-ttu-id="0c787-119">暗号化、監査、およびブロック</span><span class="sxs-lookup"><span data-stu-id="0c787-119">Encrypt, Audit and Block</span></span>|








