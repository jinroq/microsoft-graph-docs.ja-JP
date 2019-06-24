---
title: applicationTemplate リソースの種類
description: Azure AD アプリケーションギャラリーのアプリケーションを表します。
localization_priority: Normal
author: luleonpla
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 4a8e1f4cb365f86df32e32ed568aa3a96d1c090f
ms.sourcegitcommit: 7c03131291113c343a98bb0234d31bd4535a4050
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/22/2019
ms.locfileid: "35147927"
---
# <a name="applicationtemplate-resource-type"></a><span data-ttu-id="f5a5d-103">applicationTemplate リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f5a5d-103">applicationTemplate resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f5a5d-104">[AZURE AD アプリケーションギャラリー](https://docs.microsoft.com/en-us/azure/active-directory/saas-apps/tutorial-list)のアプリケーションを表します。</span><span class="sxs-lookup"><span data-stu-id="f5a5d-104">Represents an application in the [Azure AD application gallery](https://docs.microsoft.com/en-us/azure/active-directory/saas-apps/tutorial-list).</span></span>

## <a name="methods"></a><span data-ttu-id="f5a5d-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="f5a5d-105">Methods</span></span>

| <span data-ttu-id="f5a5d-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="f5a5d-106">Method</span></span>       | <span data-ttu-id="f5a5d-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="f5a5d-107">Return Type</span></span> | <span data-ttu-id="f5a5d-108">説明</span><span class="sxs-lookup"><span data-stu-id="f5a5d-108">Description</span></span> |
|:-------------|:------------|:------------|
|[<span data-ttu-id="f5a5d-109">ApplicationTemplate の一覧表示</span><span class="sxs-lookup"><span data-stu-id="f5a5d-109">List applicationTemplate</span></span>](../api/applicationtemplate-list.md)|[<span data-ttu-id="f5a5d-110">applicationTemplate</span><span class="sxs-lookup"><span data-stu-id="f5a5d-110">applicationTemplate</span></span>](applicationtemplate.md)|<span data-ttu-id="f5a5d-111">ApplicationTemplate オブジェクトのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="f5a5d-111">Retrieve a list of applicationTemplate objects.</span></span>|
| [<span data-ttu-id="f5a5d-112">ApplicationTemplate の取得</span><span class="sxs-lookup"><span data-stu-id="f5a5d-112">Get applicationTemplate</span></span>](../api/applicationtemplate-get.md) | [<span data-ttu-id="f5a5d-113">applicationTemplate</span><span class="sxs-lookup"><span data-stu-id="f5a5d-113">applicationTemplate</span></span>](applicationtemplate.md) | <span data-ttu-id="f5a5d-114">ApplicationTemplate オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="f5a5d-114">Read properties and relationships of applicationTemplate object.</span></span> |
|[<span data-ttu-id="f5a5d-115">ApplicationTemplate のインスタンス化</span><span class="sxs-lookup"><span data-stu-id="f5a5d-115">Instantiate applicationTemplate</span></span>](../api/applicationtemplate-instantiate.md)|[<span data-ttu-id="f5a5d-116">applicationServicePrincipal</span><span class="sxs-lookup"><span data-stu-id="f5a5d-116">applicationServicePrincipal</span></span>](applicationserviceprincipal.md)| <span data-ttu-id="f5a5d-117">Azure AD アプリケーションギャラリーからディレクトリにアプリケーションのインスタンスを追加します。</span><span class="sxs-lookup"><span data-stu-id="f5a5d-117">Add an instance of an application from the Azure AD application gallery into your directory.</span></span>|


## <a name="properties"></a><span data-ttu-id="f5a5d-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f5a5d-118">Properties</span></span>

| <span data-ttu-id="f5a5d-119">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f5a5d-119">Property</span></span>     | <span data-ttu-id="f5a5d-120">型</span><span class="sxs-lookup"><span data-stu-id="f5a5d-120">Type</span></span>        | <span data-ttu-id="f5a5d-121">説明</span><span class="sxs-lookup"><span data-stu-id="f5a5d-121">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="f5a5d-122">categories</span><span class="sxs-lookup"><span data-stu-id="f5a5d-122">categories</span></span>|<span data-ttu-id="f5a5d-123">String collection</span><span class="sxs-lookup"><span data-stu-id="f5a5d-123">String collection</span></span>|<span data-ttu-id="f5a5d-124">アプリケーションのカテゴリのリスト。</span><span class="sxs-lookup"><span data-stu-id="f5a5d-124">The list of categories for the application.</span></span> <span data-ttu-id="f5a5d-125">サポートされている`Collaboration`値`Business Management`は`Consumer`次`Content management`の`CRM`とおり`Data services`です`Developer services`: `E-commerce`、 `Education` `ERP` `Finance` `Health` `Human resources` `IT infrastructure` `Mail` `Management`、 `Marketing`、、、、、、、 `Media` `Productivity`、、、、および`Web design & hosting` `Project management` `Telecommunications` `Tools, Travel`</span><span class="sxs-lookup"><span data-stu-id="f5a5d-125">Supported values can be: `Collaboration`, `Business Management`, `Consumer`,`Content management`, `CRM`, `Data services`, `Developer services`, `E-commerce`, `Education`, `ERP`, `Finance`, `Health`, `Human resources`, `IT infrastructure`, `Mail`, `Management`, `Marketing`, `Media`, `Productivity`, `Project management`, `Telecommunications`, `Tools, Travel`, and `Web design & hosting`.</span></span>|
|<span data-ttu-id="f5a5d-126">description</span><span class="sxs-lookup"><span data-stu-id="f5a5d-126">description</span></span>|<span data-ttu-id="f5a5d-127">String</span><span class="sxs-lookup"><span data-stu-id="f5a5d-127">String</span></span>|<span data-ttu-id="f5a5d-128">アプリケーションの説明。</span><span class="sxs-lookup"><span data-stu-id="f5a5d-128">A description of the application.</span></span>|
|<span data-ttu-id="f5a5d-129">displayName</span><span class="sxs-lookup"><span data-stu-id="f5a5d-129">displayName</span></span>|<span data-ttu-id="f5a5d-130">String</span><span class="sxs-lookup"><span data-stu-id="f5a5d-130">String</span></span>|<span data-ttu-id="f5a5d-131">アプリケーションの名前を指定します。</span><span class="sxs-lookup"><span data-stu-id="f5a5d-131">The name of the application.</span></span>|
|<span data-ttu-id="f5a5d-132">ホームページの Url</span><span class="sxs-lookup"><span data-stu-id="f5a5d-132">homePageUrl</span></span>|<span data-ttu-id="f5a5d-133">String</span><span class="sxs-lookup"><span data-stu-id="f5a5d-133">String</span></span>|<span data-ttu-id="f5a5d-134">アプリケーションのホームページの URL。</span><span class="sxs-lookup"><span data-stu-id="f5a5d-134">The home page URL of the application.</span></span>|
|<span data-ttu-id="f5a5d-135">id</span><span class="sxs-lookup"><span data-stu-id="f5a5d-135">id</span></span>|<span data-ttu-id="f5a5d-136">文字列</span><span class="sxs-lookup"><span data-stu-id="f5a5d-136">String</span></span>| <span data-ttu-id="f5a5d-137">アプリケーションの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="f5a5d-137">Unique identifier for the application.</span></span> <span data-ttu-id="f5a5d-138">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="f5a5d-138">Read-only.</span></span>|
|<span data-ttu-id="f5a5d-139">logoUrl</span><span class="sxs-lookup"><span data-stu-id="f5a5d-139">logoUrl</span></span>|<span data-ttu-id="f5a5d-140">String</span><span class="sxs-lookup"><span data-stu-id="f5a5d-140">String</span></span>|<span data-ttu-id="f5a5d-141">このアプリケーションのロゴを取得する URL。</span><span class="sxs-lookup"><span data-stu-id="f5a5d-141">The URL to get the logo for this application.</span></span>|
|<span data-ttu-id="f5a5d-142">publisher</span><span class="sxs-lookup"><span data-stu-id="f5a5d-142">publisher</span></span>|<span data-ttu-id="f5a5d-143">String</span><span class="sxs-lookup"><span data-stu-id="f5a5d-143">String</span></span>|<span data-ttu-id="f5a5d-144">このアプリケーションの発行元の名前。</span><span class="sxs-lookup"><span data-stu-id="f5a5d-144">The name of the publisher for this application.</span></span>|
|<span data-ttu-id="f5a5d-145">Supportedプロビジョニング型</span><span class="sxs-lookup"><span data-stu-id="f5a5d-145">supportedProvisioningTypes</span></span>|<span data-ttu-id="f5a5d-146">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="f5a5d-146">String collection</span></span>|<span data-ttu-id="f5a5d-147">このアプリケーションでサポートされているプロビジョニングモードのリスト。</span><span class="sxs-lookup"><span data-stu-id="f5a5d-147">The list of provisioning modes supported by this application.</span></span> <span data-ttu-id="f5a5d-148">有効な値は`sync`です。</span><span class="sxs-lookup"><span data-stu-id="f5a5d-148">The only valid value is `sync`.</span></span>|
|<span data-ttu-id="f5a5d-149">supportedSingleSignOnModes</span><span class="sxs-lookup"><span data-stu-id="f5a5d-149">supportedSingleSignOnModes</span></span>|<span data-ttu-id="f5a5d-150">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="f5a5d-150">String collection</span></span>|<span data-ttu-id="f5a5d-151">このアプリケーションでサポートされているシングルサインオンモードの一覧です。</span><span class="sxs-lookup"><span data-stu-id="f5a5d-151">The list of single sign-on modes supported by this application.</span></span> <span data-ttu-id="f5a5d-152">サポートされて`password`いる`saml`値`external`は、 `oidc`、、です。</span><span class="sxs-lookup"><span data-stu-id="f5a5d-152">The supported values are `password`, `saml`, `external`, and `oidc`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f5a5d-153">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="f5a5d-153">Relationships</span></span>

<span data-ttu-id="f5a5d-154">なし。</span><span class="sxs-lookup"><span data-stu-id="f5a5d-154">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="f5a5d-155">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f5a5d-155">JSON representation</span></span>

<span data-ttu-id="f5a5d-156">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="f5a5d-156">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.applicationTemplate",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
    "id" : "id-value",
    "displayName" : "displayName-value",
    "homePageUrl" : "homePageUrl-value",
    "supportedSingleSignOnModes" : ["supportedSingleSignOnModes-value"],
    "logoUrl" : "logoUrl-value",
    "categories" : ["categories-value"],
    "publisher" : "publisher-value",
    "description" : "description-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "applicationTemplate resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
