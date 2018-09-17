# <a name="firewallpresharedkeyencodingmethodtype-enum-type"></a><span data-ttu-id="ab034-101">firewallPreSharedKeyEncodingMethodType 列挙型</span><span class="sxs-lookup"><span data-stu-id="ab034-101">firewallPreSharedKeyEncodingMethodType enum type</span></span>

> <span data-ttu-id="ab034-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="ab034-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ab034-103">firewallPreSharedKeyEncodingMethod に指定できる値</span><span class="sxs-lookup"><span data-stu-id="ab034-103">Possible values for firewallPreSharedKeyEncodingMethod</span></span>
## <a name="members"></a><span data-ttu-id="ab034-104">メンバー</span><span class="sxs-lookup"><span data-stu-id="ab034-104">Members</span></span>
|<span data-ttu-id="ab034-105">メンバー</span><span class="sxs-lookup"><span data-stu-id="ab034-105">Member</span></span>|<span data-ttu-id="ab034-106">値</span><span class="sxs-lookup"><span data-stu-id="ab034-106">Value</span></span>|<span data-ttu-id="ab034-107">説明</span><span class="sxs-lookup"><span data-stu-id="ab034-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ab034-108">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="ab034-108">deviceDefault</span></span>|<span data-ttu-id="ab034-109">0</span><span class="sxs-lookup"><span data-stu-id="ab034-109">0%</span></span>|<span data-ttu-id="ab034-110">Intune で設定されている値は、ユーザーが設定したデバイスの規定値よりも優先されます。</span><span class="sxs-lookup"><span data-stu-id="ab034-110">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="ab034-111">なし</span><span class="sxs-lookup"><span data-stu-id="ab034-111">none</span></span>|<span data-ttu-id="ab034-112">1</span><span class="sxs-lookup"><span data-stu-id="ab034-112">-1</span></span>|<span data-ttu-id="ab034-113">事前共有キーはエンコードされません。</span><span class="sxs-lookup"><span data-stu-id="ab034-113">Preshared key is not encoded.</span></span> <span data-ttu-id="ab034-114">その代わりに、ワイド文字形式で保存されます。</span><span class="sxs-lookup"><span data-stu-id="ab034-114">Instead, it is kept in its wide-character format</span></span>|
|<span data-ttu-id="ab034-115">utf8</span><span class="sxs-lookup"><span data-stu-id="ab034-115">utf-8</span></span>|<span data-ttu-id="ab034-116">2</span><span class="sxs-lookup"><span data-stu-id="ab034-116">-2</span></span>|<span data-ttu-id="ab034-117">UTF-8 を使用して事前共有キーをエンコードします。</span><span class="sxs-lookup"><span data-stu-id="ab034-117">Encode the preshared key using UTF-8</span></span>|








