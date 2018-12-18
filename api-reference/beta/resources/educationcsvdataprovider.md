---
title: educationCsvDataProvider リソースの種類
description: 'CSV ファイルは、入力ソースとは、学校のデータの同期プロファイルを設定するために使用します。  '
author: mmast-msft
ms.openlocfilehash: 1a816d4e176147d549381465154e35cf0a821b98
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27317900"
---
# <a name="educationcsvdataprovider-resource-type"></a><span data-ttu-id="4b01f-103">educationCsvDataProvider リソースの種類</span><span class="sxs-lookup"><span data-stu-id="4b01f-103">educationCsvDataProvider resource type</span></span>

> <span data-ttu-id="4b01f-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="4b01f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4b01f-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4b01f-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4b01f-106">CSV ファイルは、入力ソースとは、学校のデータの同期プロファイルを設定するために使用します。</span><span class="sxs-lookup"><span data-stu-id="4b01f-106">Used to set up the school data synchronization profile when CSV files are the input source.</span></span>  

<span data-ttu-id="4b01f-107">[EducationSynchronizationDataProvider](educationsynchronizationdataprovider.md)から派生します。</span><span class="sxs-lookup"><span data-stu-id="4b01f-107">Derived from [educationSynchronizationDataProvider](educationsynchronizationdataprovider.md).</span></span>

## <a name="properties"></a><span data-ttu-id="4b01f-108">Properties</span><span class="sxs-lookup"><span data-stu-id="4b01f-108">Properties</span></span>

| <span data-ttu-id="4b01f-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4b01f-109">Property</span></span> | <span data-ttu-id="4b01f-110">種類</span><span class="sxs-lookup"><span data-stu-id="4b01f-110">Type</span></span> | <span data-ttu-id="4b01f-111">説明</span><span class="sxs-lookup"><span data-stu-id="4b01f-111">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="4b01f-112">**カスタマイズ**</span><span class="sxs-lookup"><span data-stu-id="4b01f-112">**customizations**</span></span> | [<span data-ttu-id="4b01f-113">educationSynchronizationCustomizations</span><span class="sxs-lookup"><span data-stu-id="4b01f-113">educationSynchronizationCustomizations</span></span>](educationsynchronizationcustomizations.md) | <span data-ttu-id="4b01f-114">同期プロファイルを適用するオプションのカスタマイズです。</span><span class="sxs-lookup"><span data-stu-id="4b01f-114">Optional customizations to be applied to the synchronization profile.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4b01f-115">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="4b01f-115">JSON representation</span></span>

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
