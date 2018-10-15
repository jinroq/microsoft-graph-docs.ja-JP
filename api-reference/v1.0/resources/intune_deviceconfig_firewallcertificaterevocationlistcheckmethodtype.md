# <a name="firewallcertificaterevocationlistcheckmethodtype-enum-type"></a><span data-ttu-id="7d4a1-101">firewallCertificateRevocationListCheckMethodType 列挙型</span><span class="sxs-lookup"><span data-stu-id="7d4a1-101">firewallCertificateRevocationListCheckMethodType enum type</span></span>

> <span data-ttu-id="7d4a1-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="7d4a1-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7d4a1-103">FirewallCertificateRevocationListCheckMethod に対して使用可能な値</span><span class="sxs-lookup"><span data-stu-id="7d4a1-103">Possible values for firewallCertificateRevocationListCheckMethod</span></span>
## <a name="members"></a><span data-ttu-id="7d4a1-104">メンバー</span><span class="sxs-lookup"><span data-stu-id="7d4a1-104">Members</span></span>
|<span data-ttu-id="7d4a1-105">メンバー</span><span class="sxs-lookup"><span data-stu-id="7d4a1-105">Member</span></span>|<span data-ttu-id="7d4a1-106">値</span><span class="sxs-lookup"><span data-stu-id="7d4a1-106">Value</span></span>|<span data-ttu-id="7d4a1-107">説明</span><span class="sxs-lookup"><span data-stu-id="7d4a1-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7d4a1-108">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="7d4a1-108">deviceDefault</span></span>|<span data-ttu-id="7d4a1-109">0</span><span class="sxs-lookup"><span data-stu-id="7d4a1-109">0%</span></span>|<span data-ttu-id="7d4a1-110">値は Intune により未構成、ユーザーにより構成されたデバイスの規定値を上書きしないでください。</span><span class="sxs-lookup"><span data-stu-id="7d4a1-110">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="7d4a1-111">なし</span><span class="sxs-lookup"><span data-stu-id="7d4a1-111">none</span></span>|<span data-ttu-id="7d4a1-112">1</span><span class="sxs-lookup"><span data-stu-id="7d4a1-112">-1</span></span>|<span data-ttu-id="7d4a1-113">証明書失効リストをチェックしないでください。</span><span class="sxs-lookup"><span data-stu-id="7d4a1-113">Do not check certificate revocation list</span></span>|
|<span data-ttu-id="7d4a1-114">試行</span><span class="sxs-lookup"><span data-stu-id="7d4a1-114">attempt</span></span>|<span data-ttu-id="7d4a1-115">2</span><span class="sxs-lookup"><span data-stu-id="7d4a1-115">-2</span></span>|<span data-ttu-id="7d4a1-116">CRL（証明書失効リスト）チェックを試行し、証明書がチェックにより確認される場合のみ証明書を許可</span><span class="sxs-lookup"><span data-stu-id="7d4a1-116">Attempt CRL check and allow a certificate only if the certificate is confirmed by the check</span></span>|
|<span data-ttu-id="7d4a1-117">要求</span><span class="sxs-lookup"><span data-stu-id="7d4a1-117">Require</span></span>|<span data-ttu-id="7d4a1-118">3</span><span class="sxs-lookup"><span data-stu-id="7d4a1-118">"3"</span></span>|<span data-ttu-id="7d4a1-119">証明書を許可する前に正常な CRL チェックを要求</span><span class="sxs-lookup"><span data-stu-id="7d4a1-119">Require a successful CRL check before allowing a certificate</span></span>|








