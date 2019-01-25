    ---
<span data-ttu-id="ab3f1-101">タイトル:「educationIdentitySynchronizationConfiguration のリソースの種類」の説明:「すべて学校データ プロファイル id の同期設定の基本クラスを抽象化します。</span><span class="sxs-lookup"><span data-stu-id="ab3f1-101">title: "educationIdentitySynchronizationConfiguration resource type" description: "Abstract base class for all school data profile identity synchronization configurations.</span></span> <span data-ttu-id="ab3f1-102">派生クラスは、識別情報を同期するための動作を定義します。</span><span class="sxs-lookup"><span data-stu-id="ab3f1-102">The derived classes define the behavior for synchronizing identities.</span></span> <span data-ttu-id="ab3f1-103">次の派生型」</span><span class="sxs-lookup"><span data-stu-id="ab3f1-103">The following are the derived types."</span></span>
<span data-ttu-id="ab3f1-104">作成者: mmast-溺"localization_priority: 通常の ms.prod:「教育」</span><span class="sxs-lookup"><span data-stu-id="ab3f1-104">author: "mmast-msft" localization_priority: Normal ms.prod: "education"</span></span>
---

# <a name="educationidentitysynchronizationconfiguration-resource-type"></a><span data-ttu-id="ab3f1-105">educationIdentitySynchronizationConfiguration リソースの種類</span><span class="sxs-lookup"><span data-stu-id="ab3f1-105">educationIdentitySynchronizationConfiguration resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ab3f1-106">すべて学校データ プロファイルの id の同期設定の抽象基本クラスです。</span><span class="sxs-lookup"><span data-stu-id="ab3f1-106">Abstract base class for all school data profile identity synchronization configurations.</span></span> <span data-ttu-id="ab3f1-107">派生クラスは、識別情報を同期するための動作を定義します。</span><span class="sxs-lookup"><span data-stu-id="ab3f1-107">The derived classes define the behavior for synchronizing identities.</span></span> <span data-ttu-id="ab3f1-108">派生型を次に示します。</span><span class="sxs-lookup"><span data-stu-id="ab3f1-108">The following are the derived types.</span></span>

## <a name="derived-types"></a><span data-ttu-id="ab3f1-109">派生型</span><span class="sxs-lookup"><span data-stu-id="ab3f1-109">Derived types</span></span>
| <span data-ttu-id="ab3f1-110">型</span><span class="sxs-lookup"><span data-stu-id="ab3f1-110">Type</span></span> | <span data-ttu-id="ab3f1-111">説明</span><span class="sxs-lookup"><span data-stu-id="ab3f1-111">Description</span></span> |
|:-|:-|
| [<span data-ttu-id="ab3f1-112">**educationIdentityMatchingConfiguration**</span><span class="sxs-lookup"><span data-stu-id="ab3f1-112">**educationIdentityMatchingConfiguration**</span></span>](educationidentitymatchingconfiguration.md) | <span data-ttu-id="ab3f1-113">Azure Active Directory (AD の Azure) 内の既存のユーザー アカウントを一致させるには、この型を使用します。</span><span class="sxs-lookup"><span data-stu-id="ab3f1-113">Use this type to match existing user accounts in Azure Active Directory (Azure AD).</span></span> |
| [<span data-ttu-id="ab3f1-114">**educationIdentityCreationConfiguration**</span><span class="sxs-lookup"><span data-stu-id="ab3f1-114">**educationIdentityCreationConfiguration**</span></span>](educationidentitycreationconfiguration.md) | <span data-ttu-id="ab3f1-115">Azure AD で新しいユーザー アカウントを作成するのにには、この型を使用します。</span><span class="sxs-lookup"><span data-stu-id="ab3f1-115">Use this type to create new user accounts in Azure AD.</span></span> |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationidentitysynchronizationconfiguration.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
