---
title: iosSingleSignOnSettings リソースの種類
description: iOS は単一のサインオンでの Kerberos 認証の設定
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 189fb79be741bdf6b731b1e3c2b336934db8c86b
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29421320"
---
# <a name="iossinglesignonsettings-resource-type"></a><span data-ttu-id="a0644-103">iosSingleSignOnSettings リソースの種類</span><span class="sxs-lookup"><span data-stu-id="a0644-103">iosSingleSignOnSettings resource type</span></span>

> <span data-ttu-id="a0644-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="a0644-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="a0644-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a0644-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a0644-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="a0644-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a0644-107">iOS は単一のサインオンでの Kerberos 認証の設定</span><span class="sxs-lookup"><span data-stu-id="a0644-107">iOS Kerberos authentication settings for single sign-on</span></span>

## <a name="properties"></a><span data-ttu-id="a0644-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a0644-108">Properties</span></span>
|<span data-ttu-id="a0644-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a0644-109">Property</span></span>|<span data-ttu-id="a0644-110">型</span><span class="sxs-lookup"><span data-stu-id="a0644-110">Type</span></span>|<span data-ttu-id="a0644-111">説明</span><span class="sxs-lookup"><span data-stu-id="a0644-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a0644-112">allowedAppsList</span><span class="sxs-lookup"><span data-stu-id="a0644-112">allowedAppsList</span></span>|<span data-ttu-id="a0644-113">[appListItem](../resources/intune-deviceconfig-applistitem.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="a0644-113">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="a0644-114">このログインを使用するのには許可されているアプリケーションの識別子の一覧です。</span><span class="sxs-lookup"><span data-stu-id="a0644-114">List of app identifiers that are allowed to use this login.</span></span> <span data-ttu-id="a0644-115">このフィールドを省略すると、ログインは、デバイス上のすべてのアプリケーションに適用されます。</span><span class="sxs-lookup"><span data-stu-id="a0644-115">If this field is omitted, the login applies to all applications on the device.</span></span> <span data-ttu-id="a0644-116">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="a0644-116">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="a0644-117">allowedUrls</span><span class="sxs-lookup"><span data-stu-id="a0644-117">allowedUrls</span></span>|<span data-ttu-id="a0644-118">String コレクション</span><span class="sxs-lookup"><span data-stu-id="a0644-118">String collection</span></span>|<span data-ttu-id="a0644-119">このログインを使用するために一致する必要がある HTTP Url の一覧です。</span><span class="sxs-lookup"><span data-stu-id="a0644-119">List of HTTP URLs that must be matched in order to use this login.</span></span> <span data-ttu-id="a0644-120">9.0 以降、iOS でワイルドカード文字を使用することがあります。</span><span class="sxs-lookup"><span data-stu-id="a0644-120">With iOS 9.0 or later, a wildcard characters may be used.</span></span>|
|<span data-ttu-id="a0644-121">displayName</span><span class="sxs-lookup"><span data-stu-id="a0644-121">displayName</span></span>|<span data-ttu-id="a0644-122">String</span><span class="sxs-lookup"><span data-stu-id="a0644-122">String</span></span>|<span data-ttu-id="a0644-123">受信側デバイスに表示されるログインの設定の表示名。</span><span class="sxs-lookup"><span data-stu-id="a0644-123">The display name of login settings shown on the receiving device.</span></span>|
|<span data-ttu-id="a0644-124">kerberosPrincipalName</span><span class="sxs-lookup"><span data-stu-id="a0644-124">kerberosPrincipalName</span></span>|<span data-ttu-id="a0644-125">String</span><span class="sxs-lookup"><span data-stu-id="a0644-125">String</span></span>|<span data-ttu-id="a0644-126">Kerberos プリンシパルの名前です。</span><span class="sxs-lookup"><span data-stu-id="a0644-126">A Kerberos principal name.</span></span> <span data-ttu-id="a0644-127">指定しない場合、プロファイルのインストール時にいずれかの入力が求められます。</span><span class="sxs-lookup"><span data-stu-id="a0644-127">If not provided, the user is prompted for one during profile installation.</span></span>|
|<span data-ttu-id="a0644-128">kerberosRealm</span><span class="sxs-lookup"><span data-stu-id="a0644-128">kerberosRealm</span></span>|<span data-ttu-id="a0644-129">String</span><span class="sxs-lookup"><span data-stu-id="a0644-129">String</span></span>|<span data-ttu-id="a0644-130">Kerberos レルムの名前です。</span><span class="sxs-lookup"><span data-stu-id="a0644-130">A Kerberos realm name.</span></span> <span data-ttu-id="a0644-131">大文字小文字を区別します。</span><span class="sxs-lookup"><span data-stu-id="a0644-131">Case sensitive.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a0644-132">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="a0644-132">Relationships</span></span>
<span data-ttu-id="a0644-133">なし</span><span class="sxs-lookup"><span data-stu-id="a0644-133">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a0644-134">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a0644-134">JSON Representation</span></span>
<span data-ttu-id="a0644-135">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="a0644-135">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosSingleSignOnSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosSingleSignOnSettings",
  "allowedAppsList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "String",
      "publisher": "String",
      "appStoreUrl": "String",
      "appId": "String"
    }
  ],
  "allowedUrls": [
    "String"
  ],
  "displayName": "String",
  "kerberosPrincipalName": "String",
  "kerberosRealm": "String"
}
```




