---
title: applicationServicePrincipal リソースの種類
description: アプリケーションと servicePrincipal の組み合わせ。
localization_priority: Normal
author: luleonpla
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: c3a6d0d1017f89587f1f826c4225eefc51dc5edb
ms.sourcegitcommit: 7c03131291113c343a98bb0234d31bd4535a4050
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/22/2019
ms.locfileid: "35147928"
---
# <a name="applicationserviceprincipal-resource-type"></a><span data-ttu-id="4ad94-103">applicationServicePrincipal リソースの種類</span><span class="sxs-lookup"><span data-stu-id="4ad94-103">applicationServicePrincipal resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4ad94-104">Azure AD アプリケーションギャラリーからアプリケーションのインスタンスが追加されると、 [application](../resources/application.md)および[serviceprincipal](../resources/serviceprincipal.md)オブジェクトがディレクトリに作成されます。</span><span class="sxs-lookup"><span data-stu-id="4ad94-104">When an instance of an application from the Azure AD application gallery is added, [application](../resources/application.md) and [servicePrincipal](../resources/serviceprincipal.md) objects are created in the directory.</span></span> <span data-ttu-id="4ad94-105">**Applicationserviceprincipal**は、 **Application**と**serviceprincipal**オブジェクトの連結を表します。</span><span class="sxs-lookup"><span data-stu-id="4ad94-105">The **applicationServicePrincipal** represents the concatenation of the **application** and **servicePrincipal** object.</span></span>

## <a name="methods"></a><span data-ttu-id="4ad94-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="4ad94-106">Methods</span></span>

<span data-ttu-id="4ad94-107">None</span><span class="sxs-lookup"><span data-stu-id="4ad94-107">None</span></span>

## <a name="properties"></a><span data-ttu-id="4ad94-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4ad94-108">Properties</span></span>

| <span data-ttu-id="4ad94-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4ad94-109">Property</span></span> | <span data-ttu-id="4ad94-110">型</span><span class="sxs-lookup"><span data-stu-id="4ad94-110">Type</span></span>        | <span data-ttu-id="4ad94-111">説明</span><span class="sxs-lookup"><span data-stu-id="4ad94-111">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="4ad94-112">application</span><span class="sxs-lookup"><span data-stu-id="4ad94-112">application</span></span>|[<span data-ttu-id="4ad94-113">application</span><span class="sxs-lookup"><span data-stu-id="4ad94-113">application</span></span>](../resources/application.md)|<span data-ttu-id="4ad94-114">Azure Active Directory に登録されているアプリケーションを表します。</span><span class="sxs-lookup"><span data-stu-id="4ad94-114">Represents an application registered in Azure Active Directory.</span></span>|
|<span data-ttu-id="4ad94-115">servicePrincipal</span><span class="sxs-lookup"><span data-stu-id="4ad94-115">servicePrincipal</span></span>|[<span data-ttu-id="4ad94-116">servicePrincipal</span><span class="sxs-lookup"><span data-stu-id="4ad94-116">servicePrincipal</span></span>](../resources/serviceprincipal.md)|<span data-ttu-id="4ad94-117">ディレクトリ内のアプリケーションのインスタンスを表します。</span><span class="sxs-lookup"><span data-stu-id="4ad94-117">Represents an instance of an application in a directory.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4ad94-118">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="4ad94-118">Relationships</span></span>

<span data-ttu-id="4ad94-119">なし</span><span class="sxs-lookup"><span data-stu-id="4ad94-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4ad94-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="4ad94-120">JSON representation</span></span>

<span data-ttu-id="4ad94-121">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="4ad94-121">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.applicationServicePrincipal",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
   "servicePrincipal": {"@odata.type":"microsoft.graph.servicePrincipal"},
   "application": {"@odata.type":"microsoft.graph.application"}
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "applicationServicePrincipal resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
