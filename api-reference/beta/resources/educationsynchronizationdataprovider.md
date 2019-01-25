---
title: educationSynchronizationDataProvider リソースの種類
description: 'ソース SIS のスキーマを表します。 これにより、受信データを Azure Active Directory (AD の Azure) スキーマにマップする方法を把握するシステムです。 '
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: f592e75a3a6df1728839494ee41ac28065450d60
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29515497"
---
# <a name="educationsynchronizationdataprovider-resource-type"></a><span data-ttu-id="2036d-104">educationSynchronizationDataProvider リソースの種類</span><span class="sxs-lookup"><span data-stu-id="2036d-104">educationSynchronizationDataProvider resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2036d-105">ソース SIS のスキーマを表します。</span><span class="sxs-lookup"><span data-stu-id="2036d-105">Represents the source SIS schema.</span></span> <span data-ttu-id="2036d-106">これにより、受信データを Azure Active Directory (AD の Azure) スキーマにマップする方法を把握するシステムです。</span><span class="sxs-lookup"><span data-stu-id="2036d-106">This allows the system to know how to map the incoming data to the Azure Active Directory (Azure AD) schema.</span></span>

> <span data-ttu-id="2036d-107">**注:** この複合型は抽象です。</span><span class="sxs-lookup"><span data-stu-id="2036d-107">**Note:** This complex type is abstract.</span></span> <span data-ttu-id="2036d-108">特定の種類の一覧のデータ プロバイダーを参照してください。</span><span class="sxs-lookup"><span data-stu-id="2036d-108">Refer to the specific types of data providers listed.</span></span>

## <a name="derived-types"></a><span data-ttu-id="2036d-109">派生型</span><span class="sxs-lookup"><span data-stu-id="2036d-109">Derived types</span></span>
| <span data-ttu-id="2036d-110">型</span><span class="sxs-lookup"><span data-stu-id="2036d-110">Type</span></span> | <span data-ttu-id="2036d-111">説明</span><span class="sxs-lookup"><span data-stu-id="2036d-111">Description</span></span> |
|:-|:-|:-|
| [<span data-ttu-id="2036d-112">educationcsvdataprovider</span><span class="sxs-lookup"><span data-stu-id="2036d-112">educationcsvdataprovider</span></span>](educationcsvdataprovider.md) | <span data-ttu-id="2036d-113">入力ソースとして CSV ファイルを使用します。</span><span class="sxs-lookup"><span data-stu-id="2036d-113">Used with CSV files as the input source.</span></span> |
| [<span data-ttu-id="2036d-114">educationpowerschooldataprovider</span><span class="sxs-lookup"><span data-stu-id="2036d-114">educationpowerschooldataprovider</span></span>](educationpowerschooldataprovider.md) | <span data-ttu-id="2036d-115">入力ソースとして PowerSchool を使用します。</span><span class="sxs-lookup"><span data-stu-id="2036d-115">Used with PowerSchool as the input source.</span></span> |
| [<span data-ttu-id="2036d-116">educationonerosterapidataprovider</span><span class="sxs-lookup"><span data-stu-id="2036d-116">educationonerosterapidataprovider</span></span>](educationonerosterapidataprovider.md) | <span data-ttu-id="2036d-117">入力ソースとして、OneRoster API を使用します。</span><span class="sxs-lookup"><span data-stu-id="2036d-117">Used with OneRoster API as the input source.</span></span> |

## <a name="properties"></a><span data-ttu-id="2036d-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2036d-118">Properties</span></span>

<span data-ttu-id="2036d-119">この型でのプロパティはありません。</span><span class="sxs-lookup"><span data-stu-id="2036d-119">No properties are exposed by this type.</span></span>
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationsynchronizationdataprovider.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
