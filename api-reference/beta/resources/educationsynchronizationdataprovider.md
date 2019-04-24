---
title: educationSynchronizationDataProvider リソースの種類
description: 'ソース SIS スキーマを表します。 これにより、システムは、受信データを azure Active Directory (azure AD) スキーマにマップする方法を知ることができます。 '
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: f592e75a3a6df1728839494ee41ac28065450d60
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32507040"
---
# <a name="educationsynchronizationdataprovider-resource-type"></a><span data-ttu-id="f25b2-104">educationSynchronizationDataProvider リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f25b2-104">educationSynchronizationDataProvider resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f25b2-105">ソース SIS スキーマを表します。</span><span class="sxs-lookup"><span data-stu-id="f25b2-105">Represents the source SIS schema.</span></span> <span data-ttu-id="f25b2-106">これにより、システムは、受信データを azure Active Directory (azure AD) スキーマにマップする方法を知ることができます。</span><span class="sxs-lookup"><span data-stu-id="f25b2-106">This allows the system to know how to map the incoming data to the Azure Active Directory (Azure AD) schema.</span></span>

> <span data-ttu-id="f25b2-107">**注:** この複合型は抽象型です。</span><span class="sxs-lookup"><span data-stu-id="f25b2-107">**Note:** This complex type is abstract.</span></span> <span data-ttu-id="f25b2-108">記載されている特定の種類のデータプロバイダーを参照してください。</span><span class="sxs-lookup"><span data-stu-id="f25b2-108">Refer to the specific types of data providers listed.</span></span>

## <a name="derived-types"></a><span data-ttu-id="f25b2-109">派生型</span><span class="sxs-lookup"><span data-stu-id="f25b2-109">Derived types</span></span>
| <span data-ttu-id="f25b2-110">型</span><span class="sxs-lookup"><span data-stu-id="f25b2-110">Type</span></span> | <span data-ttu-id="f25b2-111">説明</span><span class="sxs-lookup"><span data-stu-id="f25b2-111">Description</span></span> |
|:-|:-|:-|
| [<span data-ttu-id="f25b2-112">educationcsvdataprovider</span><span class="sxs-lookup"><span data-stu-id="f25b2-112">educationcsvdataprovider</span></span>](educationcsvdataprovider.md) | <span data-ttu-id="f25b2-113">入力ソースとして CSV ファイルで使用されます。</span><span class="sxs-lookup"><span data-stu-id="f25b2-113">Used with CSV files as the input source.</span></span> |
| [<span data-ttu-id="f25b2-114">educationpowerschooldataprovider</span><span class="sxs-lookup"><span data-stu-id="f25b2-114">educationpowerschooldataprovider</span></span>](educationpowerschooldataprovider.md) | <span data-ttu-id="f25b2-115">入力ソースとして powerschool を使用します。</span><span class="sxs-lookup"><span data-stu-id="f25b2-115">Used with PowerSchool as the input source.</span></span> |
| [<span data-ttu-id="f25b2-116">educationonerosterapidataprovider</span><span class="sxs-lookup"><span data-stu-id="f25b2-116">educationonerosterapidataprovider</span></span>](educationonerosterapidataprovider.md) | <span data-ttu-id="f25b2-117">入力ソースとして OneRoster API で使用されます。</span><span class="sxs-lookup"><span data-stu-id="f25b2-117">Used with OneRoster API as the input source.</span></span> |

## <a name="properties"></a><span data-ttu-id="f25b2-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f25b2-118">Properties</span></span>

<span data-ttu-id="f25b2-119">この種類のプロパティは公開されません。</span><span class="sxs-lookup"><span data-stu-id="f25b2-119">No properties are exposed by this type.</span></span>
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationsynchronizationdataprovider.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
