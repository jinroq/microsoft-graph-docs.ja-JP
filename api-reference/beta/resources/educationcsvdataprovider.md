---
title: educationCsvDataProvider リソースの種類
description: 'CSV ファイルは、入力ソースとは、学校のデータの同期プロファイルを設定するために使用します。  '
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 19ef77671f862a0b59b5697b76bb54dc20e42856
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27952756"
---
# <a name="educationcsvdataprovider-resource-type"></a><span data-ttu-id="fe142-103">educationCsvDataProvider リソースの種類</span><span class="sxs-lookup"><span data-stu-id="fe142-103">educationCsvDataProvider resource type</span></span>

> <span data-ttu-id="fe142-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="fe142-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fe142-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fe142-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="fe142-106">CSV ファイルは、入力ソースとは、学校のデータの同期プロファイルを設定するために使用します。</span><span class="sxs-lookup"><span data-stu-id="fe142-106">Used to set up the school data synchronization profile when CSV files are the input source.</span></span>  

<span data-ttu-id="fe142-107">[EducationSynchronizationDataProvider](educationsynchronizationdataprovider.md)から派生します。</span><span class="sxs-lookup"><span data-stu-id="fe142-107">Derived from [educationSynchronizationDataProvider](educationsynchronizationdataprovider.md).</span></span>

## <a name="properties"></a><span data-ttu-id="fe142-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fe142-108">Properties</span></span>

| <span data-ttu-id="fe142-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fe142-109">Property</span></span> | <span data-ttu-id="fe142-110">種類</span><span class="sxs-lookup"><span data-stu-id="fe142-110">Type</span></span> | <span data-ttu-id="fe142-111">説明</span><span class="sxs-lookup"><span data-stu-id="fe142-111">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="fe142-112">**カスタマイズ**</span><span class="sxs-lookup"><span data-stu-id="fe142-112">**customizations**</span></span> | [<span data-ttu-id="fe142-113">educationSynchronizationCustomizations</span><span class="sxs-lookup"><span data-stu-id="fe142-113">educationSynchronizationCustomizations</span></span>](educationsynchronizationcustomizations.md) | <span data-ttu-id="fe142-114">同期プロファイルを適用するオプションのカスタマイズです。</span><span class="sxs-lookup"><span data-stu-id="fe142-114">Optional customizations to be applied to the synchronization profile.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="fe142-115">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="fe142-115">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "#microsoft.graph.educationCsvDataProvider"
}-->

```json
{
    "@odata.type": "#microsoft.graph.educationCsvDataProvider",
    "customizations": { "@odata.type": "microsoft.graph.educationSynchronizationCustomizations" }
}
```
