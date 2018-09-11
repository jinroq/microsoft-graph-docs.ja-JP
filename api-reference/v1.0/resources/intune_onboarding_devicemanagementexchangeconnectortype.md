# <a name="devicemanagementexchangeconnectortype-enum-type"></a><span data-ttu-id="aa01e-101">deviceManagementExchangeConnectorType 列挙型</span><span class="sxs-lookup"><span data-stu-id="aa01e-101">deviceManagementExchangeConnectorType enum type</span></span>

> <span data-ttu-id="aa01e-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="aa01e-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="aa01e-103">Exchange コネクタの種類。</span><span class="sxs-lookup"><span data-stu-id="aa01e-103">The type of Exchange Connector Configured.</span></span>
## <a name="members"></a><span data-ttu-id="aa01e-104">メンバー</span><span class="sxs-lookup"><span data-stu-id="aa01e-104">Members</span></span>
|<span data-ttu-id="aa01e-105">メンバー</span><span class="sxs-lookup"><span data-stu-id="aa01e-105">Member</span></span>|<span data-ttu-id="aa01e-106">値</span><span class="sxs-lookup"><span data-stu-id="aa01e-106">Value</span></span>|<span data-ttu-id="aa01e-107">説明</span><span class="sxs-lookup"><span data-stu-id="aa01e-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aa01e-108">onPremises</span><span class="sxs-lookup"><span data-stu-id="aa01e-108">On-premises</span></span>|<span data-ttu-id="aa01e-109">0</span><span class="sxs-lookup"><span data-stu-id="aa01e-109">0%</span></span>|<span data-ttu-id="aa01e-110">オンプレミスの Exchange 環境に接続します。</span><span class="sxs-lookup"><span data-stu-id="aa01e-110">Connects to on-premises Exchange Environment.</span></span>|
|<span data-ttu-id="aa01e-111">Hosted</span><span class="sxs-lookup"><span data-stu-id="aa01e-111">Hosted</span></span>|<span data-ttu-id="aa01e-112">1</span><span class="sxs-lookup"><span data-stu-id="aa01e-112">-1</span></span>|<span data-ttu-id="aa01e-113">O365 マルチ テナント型の Exchange 環境に接続します。</span><span class="sxs-lookup"><span data-stu-id="aa01e-113">Connects to O365 multi-tenant Exchange environment</span></span>|
|<span data-ttu-id="aa01e-114">serviceToService</span><span class="sxs-lookup"><span data-stu-id="aa01e-114">Service-to-service</span></span>|<span data-ttu-id="aa01e-115">2</span><span class="sxs-lookup"><span data-stu-id="aa01e-115">-2</span></span>|<span data-ttu-id="aa01e-116">Intune サービスが O365 マルチ テナント型の Exchange 環境に直接接続します。</span><span class="sxs-lookup"><span data-stu-id="aa01e-116">Intune Service connects directly to O365 multi-tenant Exchange environment</span></span>|
|<span data-ttu-id="aa01e-117">dedicated</span><span class="sxs-lookup"><span data-stu-id="aa01e-117">Dedicated</span></span>|<span data-ttu-id="aa01e-118">3</span><span class="sxs-lookup"><span data-stu-id="aa01e-118">"3"</span></span>|<span data-ttu-id="aa01e-119">O365 専用の Exchange 環境に接続します。</span><span class="sxs-lookup"><span data-stu-id="aa01e-119">Connects to O365 Dedicated Exchange environment.</span></span>|








