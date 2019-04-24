    ---
<span data-ttu-id="f818e-101">title: "educationIdentitySynchronizationConfiguration resource type" description: "すべての学校データプロファイル id 同期構成の抽象基本クラス。</span><span class="sxs-lookup"><span data-stu-id="f818e-101">title: "educationIdentitySynchronizationConfiguration resource type" description: "Abstract base class for all school data profile identity synchronization configurations.</span></span> <span data-ttu-id="f818e-102">派生クラスは、id を同期するための動作を定義します。</span><span class="sxs-lookup"><span data-stu-id="f818e-102">The derived classes define the behavior for synchronizing identities.</span></span> <span data-ttu-id="f818e-103">派生型の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="f818e-103">The following are the derived types."</span></span>
<span data-ttu-id="f818e-104">著者: "mmast-msft" 送受信: 通常の ms 製品: "教育"</span><span class="sxs-lookup"><span data-stu-id="f818e-104">author: "mmast-msft" localization_priority: Normal ms.prod: "education"</span></span>
---

# <a name="educationidentitysynchronizationconfiguration-resource-type"></a><span data-ttu-id="f818e-105">educationIdentitySynchronizationConfiguration リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f818e-105">educationIdentitySynchronizationConfiguration resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f818e-106">すべての学校データプロファイル id 同期構成の抽象基本クラス。</span><span class="sxs-lookup"><span data-stu-id="f818e-106">Abstract base class for all school data profile identity synchronization configurations.</span></span> <span data-ttu-id="f818e-107">派生クラスは、id を同期するための動作を定義します。</span><span class="sxs-lookup"><span data-stu-id="f818e-107">The derived classes define the behavior for synchronizing identities.</span></span> <span data-ttu-id="f818e-108">派生型を次に示します。</span><span class="sxs-lookup"><span data-stu-id="f818e-108">The following are the derived types.</span></span>

## <a name="derived-types"></a><span data-ttu-id="f818e-109">派生型</span><span class="sxs-lookup"><span data-stu-id="f818e-109">Derived types</span></span>
| <span data-ttu-id="f818e-110">型</span><span class="sxs-lookup"><span data-stu-id="f818e-110">Type</span></span> | <span data-ttu-id="f818e-111">説明</span><span class="sxs-lookup"><span data-stu-id="f818e-111">Description</span></span> |
|:-|:-|
| [<span data-ttu-id="f818e-112">**educationIdentityMatchingConfiguration**</span><span class="sxs-lookup"><span data-stu-id="f818e-112">**educationIdentityMatchingConfiguration**</span></span>](educationidentitymatchingconfiguration.md) | <span data-ttu-id="f818e-113">この種類を使用して、azure Active Directory (azure AD) の既存のユーザーアカウントと照合します。</span><span class="sxs-lookup"><span data-stu-id="f818e-113">Use this type to match existing user accounts in Azure Active Directory (Azure AD).</span></span> |
| [<span data-ttu-id="f818e-114">**educationIdentityCreationConfiguration**</span><span class="sxs-lookup"><span data-stu-id="f818e-114">**educationIdentityCreationConfiguration**</span></span>](educationidentitycreationconfiguration.md) | <span data-ttu-id="f818e-115">この種類を使用して、Azure AD で新しいユーザーアカウントを作成します。</span><span class="sxs-lookup"><span data-stu-id="f818e-115">Use this type to create new user accounts in Azure AD.</span></span> |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationidentitysynchronizationconfiguration.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
