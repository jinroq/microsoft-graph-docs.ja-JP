# <a name="managedappdataencryptiontype-enum-type"></a><span data-ttu-id="4166c-101">managedAppDataEncryptionType 列挙型</span><span class="sxs-lookup"><span data-stu-id="4166c-101">managedAppDataEncryptionType enum type</span></span>

> <span data-ttu-id="4166c-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="4166c-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4166c-103">マネージ アプリのデータの暗号化レベルを示します</span><span class="sxs-lookup"><span data-stu-id="4166c-103">Represents the level to which app data is encrypted for managed apps</span></span>
## <a name="members"></a><span data-ttu-id="4166c-104">メンバー</span><span class="sxs-lookup"><span data-stu-id="4166c-104">Members</span></span>
|<span data-ttu-id="4166c-105">メンバー</span><span class="sxs-lookup"><span data-stu-id="4166c-105">Member</span></span>|<span data-ttu-id="4166c-106">値</span><span class="sxs-lookup"><span data-stu-id="4166c-106">Value</span></span>|<span data-ttu-id="4166c-107">説明</span><span class="sxs-lookup"><span data-stu-id="4166c-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4166c-108">useDeviceSettings</span><span class="sxs-lookup"><span data-stu-id="4166c-108">useDeviceSettings</span></span>|<span data-ttu-id="4166c-109">0</span><span class="sxs-lookup"><span data-stu-id="4166c-109">0%</span></span>|<span data-ttu-id="4166c-110">アプリのデータはデバイスのデフォルト設定に基づき暗号化されている</span><span class="sxs-lookup"><span data-stu-id="4166c-110">App data is encrypted based on the default settings on the device.</span></span>|
|<span data-ttu-id="4166c-111">afterDeviceRestart</span><span class="sxs-lookup"><span data-stu-id="4166c-111">afterDeviceRestart</span></span>|<span data-ttu-id="4166c-112">1</span><span class="sxs-lookup"><span data-stu-id="4166c-112">-1</span></span>|<span data-ttu-id="4166c-113">アプリのデータはデバイスを再起動すると暗号化される</span><span class="sxs-lookup"><span data-stu-id="4166c-113">App data is encrypted when the device is restarted.</span></span>|
|<span data-ttu-id="4166c-114">whenDeviceLockedExceptOpenFiles</span><span class="sxs-lookup"><span data-stu-id="4166c-114">whenDeviceLockedExceptOpenFiles</span></span>|<span data-ttu-id="4166c-115">2</span><span class="sxs-lookup"><span data-stu-id="4166c-115">-2</span></span>|<span data-ttu-id="4166c-116">このポリシーに関連付けられたアプリのデータは、オープンしているファイルのデータを除き、デバイスがロックされると暗号化される</span><span class="sxs-lookup"><span data-stu-id="4166c-116">App data associated with this policy is encrypted when the device is locked, except data in files that are open</span></span>|
|<span data-ttu-id="4166c-117">whenDeviceLocked</span><span class="sxs-lookup"><span data-stu-id="4166c-117">whenDeviceLocked</span></span>|<span data-ttu-id="4166c-118">3</span><span class="sxs-lookup"><span data-stu-id="4166c-118">"3"</span></span>|<span data-ttu-id="4166c-119">このポリシーに関連付けられたアプリのデータは、デバイスがロックされると暗号化される</span><span class="sxs-lookup"><span data-stu-id="4166c-119">App data associated with this policy is encrypted when the device is locked</span></span>|








