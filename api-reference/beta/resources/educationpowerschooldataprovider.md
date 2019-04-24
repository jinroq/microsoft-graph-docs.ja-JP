---
title: educationPowerSchoolDataProvider リソース
description: powerschool が入力ソースとして使用されている場合に、学校データ同期プロファイルを設定するために使用されます。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 2469a99b8acbfa1bd4e5167cf67caa102fa9422e
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32507127"
---
# <a name="educationpowerschooldataprovider-resource"></a><span data-ttu-id="9d4d4-103">educationPowerSchoolDataProvider リソース</span><span class="sxs-lookup"><span data-stu-id="9d4d4-103">educationPowerSchoolDataProvider resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9d4d4-104">[powerschool](https://www.powerschool.com/solutions/student-information-system-sis/)が入力ソースとして使用されている場合に、学校データ同期プロファイルを設定するために使用されます。</span><span class="sxs-lookup"><span data-stu-id="9d4d4-104">Used to set up the school data synchronization profile when [PowerSchool](https://www.powerschool.com/solutions/student-information-system-sis/) is used as the input source.</span></span>

<span data-ttu-id="9d4d4-105">[educationSynchronizationDataProvider](educationsynchronizationdataprovider.md)から派生します。</span><span class="sxs-lookup"><span data-stu-id="9d4d4-105">Derived from [educationSynchronizationDataProvider](educationsynchronizationdataprovider.md).</span></span>

## <a name="properties"></a><span data-ttu-id="9d4d4-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9d4d4-106">Properties</span></span>

| <span data-ttu-id="9d4d4-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9d4d4-107">Property</span></span> | <span data-ttu-id="9d4d4-108">型</span><span class="sxs-lookup"><span data-stu-id="9d4d4-108">Type</span></span> | <span data-ttu-id="9d4d4-109">説明</span><span class="sxs-lookup"><span data-stu-id="9d4d4-109">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="9d4d4-110">**connectionurl**</span><span class="sxs-lookup"><span data-stu-id="9d4d4-110">**connectionUrl**</span></span> | <span data-ttu-id="9d4d4-111">String</span><span class="sxs-lookup"><span data-stu-id="9d4d4-111">String</span></span> | <span data-ttu-id="9d4d4-112">powerschool インスタンスへの接続 URL。</span><span class="sxs-lookup"><span data-stu-id="9d4d4-112">The connection URL to the PowerSchool instance.</span></span> |
| <span data-ttu-id="9d4d4-113">**clientId**</span><span class="sxs-lookup"><span data-stu-id="9d4d4-113">**clientId**</span></span> | <span data-ttu-id="9d4d4-114">String</span><span class="sxs-lookup"><span data-stu-id="9d4d4-114">String</span></span> |  <span data-ttu-id="9d4d4-115">powerschool への接続に使用されるクライアント ID。</span><span class="sxs-lookup"><span data-stu-id="9d4d4-115">The client ID used to connect to PowerSchool.</span></span> |
| <span data-ttu-id="9d4d4-116">**clientSecret**</span><span class="sxs-lookup"><span data-stu-id="9d4d4-116">**clientSecret**</span></span> | <span data-ttu-id="9d4d4-117">String</span><span class="sxs-lookup"><span data-stu-id="9d4d4-117">String</span></span> |  <span data-ttu-id="9d4d4-118">powerschool インスタンスへの接続を認証するクライアントシークレット。</span><span class="sxs-lookup"><span data-stu-id="9d4d4-118">The client secret to authenticate the connection to the PowerSchool instance.</span></span> |
| <span data-ttu-id="9d4d4-119">**schoolsIds**</span><span class="sxs-lookup"><span data-stu-id="9d4d4-119">**schoolsIds**</span></span> | <span data-ttu-id="9d4d4-120">String collection</span><span class="sxs-lookup"><span data-stu-id="9d4d4-120">String collection</span></span> |  <span data-ttu-id="9d4d4-121">同期する教育機関のリスト。</span><span class="sxs-lookup"><span data-stu-id="9d4d4-121">The list of schools to sync.</span></span> |
| <span data-ttu-id="9d4d4-122">**schoolYear**</span><span class="sxs-lookup"><span data-stu-id="9d4d4-122">**schoolYear**</span></span> | <span data-ttu-id="9d4d4-123">String</span><span class="sxs-lookup"><span data-stu-id="9d4d4-123">String</span></span> |  <span data-ttu-id="9d4d4-124">同期する学校の年。</span><span class="sxs-lookup"><span data-stu-id="9d4d4-124">The school year to sync.</span></span> |
| <span data-ttu-id="9d4d4-125">**allowTeachersInMultipleSchools**</span><span class="sxs-lookup"><span data-stu-id="9d4d4-125">**allowTeachersInMultipleSchools**</span></span> | <span data-ttu-id="9d4d4-126">Boolean</span><span class="sxs-lookup"><span data-stu-id="9d4d4-126">Boolean</span></span> |  <span data-ttu-id="9d4d4-127">単一の学生または教師に対して、ソースに複数の識別子があるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="9d4d4-127">Indicates whether the source has multiple identifiers for a single student or teacher.</span></span> |
| <span data-ttu-id="9d4d4-128">**ユーザー**</span><span class="sxs-lookup"><span data-stu-id="9d4d4-128">**customizations**</span></span> | [<span data-ttu-id="9d4d4-129">educationSynchronizationCustomizations</span><span class="sxs-lookup"><span data-stu-id="9d4d4-129">educationSynchronizationCustomizations</span></span>](educationsynchronizationcustomizations.md) | <span data-ttu-id="9d4d4-130">同期プロファイルに適用されるカスタマイズ (オプション)。</span><span class="sxs-lookup"><span data-stu-id="9d4d4-130">Optional customization to be applied to the synchronization profile.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9d4d4-131">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="9d4d4-131">JSON representation</span></span>
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationPowerSchoolDataProvider"
}-->

```json
{
    "@odata.type": "microsoft.graph.educationPowerSchoolDataProvider",
    "connectionUrl": "String",
    "clientId": "String",
    "clientSecret": "String",
    "schoolsids": ["String"],
    "schoolYear": "String",
    "allowTeachersInMultipleSchools": "Boolean",
    "customizations": { "@odata.type": "microsoft.graph.educationSynchronizationCustomizations" }
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationpowerschooldataprovider.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
