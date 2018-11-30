---
title: educationIdentityMatchingConfiguration リソースの種類
description: 学校のデータのプロファイルの id を一致させるための設定を定義します。 これらの id には、生徒と教師が含まれます。 これらの設定に基づいて、ユーザーがディレクトリで更新されます。
ms.openlocfilehash: b189735340c121a56c48ae21518989cf8e1634f9
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27073618"
---
## <a name="educationidentitymatchingconfiguration-resource-type"></a><span data-ttu-id="a1400-105">educationIdentityMatchingConfiguration リソースの種類</span><span class="sxs-lookup"><span data-stu-id="a1400-105">educationIdentityMatchingConfiguration resource type</span></span>

> <span data-ttu-id="a1400-106">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="a1400-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a1400-107">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a1400-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a1400-108">学校のデータのプロファイルの id を一致させるための設定を定義します。</span><span class="sxs-lookup"><span data-stu-id="a1400-108">Defines the settings for matching school data profile identities.</span></span> <span data-ttu-id="a1400-109">これらの id には、生徒と教師が含まれます。</span><span class="sxs-lookup"><span data-stu-id="a1400-109">These identities include students and teachers.</span></span> <span data-ttu-id="a1400-110">これらの設定に基づいて、ユーザーがディレクトリで更新されます。</span><span class="sxs-lookup"><span data-stu-id="a1400-110">Based on these settings, the users will be updated in the directory.</span></span>

> <span data-ttu-id="a1400-111">**注:** このリソースが選択されている場合は、ユーザーは作成されません。</span><span class="sxs-lookup"><span data-stu-id="a1400-111">**Note:** No users are created when this resource is selected.</span></span>

## <a name="properties"></a><span data-ttu-id="a1400-112">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a1400-112">Properties</span></span>

| <span data-ttu-id="a1400-113">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a1400-113">Property</span></span> | <span data-ttu-id="a1400-114">型</span><span class="sxs-lookup"><span data-stu-id="a1400-114">Type</span></span> | <span data-ttu-id="a1400-115">説明</span><span class="sxs-lookup"><span data-stu-id="a1400-115">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="a1400-116">**matchingOptions**</span><span class="sxs-lookup"><span data-stu-id="a1400-116">**matchingOptions**</span></span> | <span data-ttu-id="a1400-117">[educationIdentityMatchingOptions](educationidentitymatchingoptions.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="a1400-117">[educationIdentityMatchingOptions](educationidentitymatchingoptions.md) collection</span></span> | <span data-ttu-id="a1400-118">ユーザー アカウントを更新するユーザーを一意に識別に使用するオプションの間のマッピングです。</span><span class="sxs-lookup"><span data-stu-id="a1400-118">Mapping between the user account and the options to use to uniquely identify the user to update.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="a1400-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a1400-119">JSON representation</span></span>
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "#microsoft.graph.educationIdentityMatchingConfiguration"
}-->

```json
{
    "@odata.type": "#microsoft.graph.educationIdentityMatchingConfiguration",
    "matchingOptions": [
        {
            "appliesTo": {"@odata.type": "#microsoft.graph.educationUserRole"},
            "sourcePropertyName": "String",
            "targetPropertyName": "String",
            "targetDomain": "String"
        }
    ]
}
```
