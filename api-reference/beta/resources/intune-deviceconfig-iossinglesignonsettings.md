---
title: iosSingleSignOnSettings リソースの種類
description: シングルサインオンの iOS Kerberos 認証設定
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 75c63454442510b62fe4c7391d4e1a5b86164bca
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33946400"
---
# <a name="iossinglesignonsettings-resource-type"></a><span data-ttu-id="0dfc4-103">iosSingleSignOnSettings リソースの種類</span><span class="sxs-lookup"><span data-stu-id="0dfc4-103">iosSingleSignOnSettings resource type</span></span>

> <span data-ttu-id="0dfc4-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0dfc4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0dfc4-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="0dfc4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0dfc4-106">シングルサインオンの iOS Kerberos 認証設定</span><span class="sxs-lookup"><span data-stu-id="0dfc4-106">iOS Kerberos authentication settings for single sign-on</span></span>

## <a name="properties"></a><span data-ttu-id="0dfc4-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0dfc4-107">Properties</span></span>
|<span data-ttu-id="0dfc4-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0dfc4-108">Property</span></span>|<span data-ttu-id="0dfc4-109">型</span><span class="sxs-lookup"><span data-stu-id="0dfc4-109">Type</span></span>|<span data-ttu-id="0dfc4-110">説明</span><span class="sxs-lookup"><span data-stu-id="0dfc4-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0dfc4-111">allowedAppsList プロパティ</span><span class="sxs-lookup"><span data-stu-id="0dfc4-111">allowedAppsList</span></span>|<span data-ttu-id="0dfc4-112">[appListItem](../resources/intune-deviceconfig-applistitem.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="0dfc4-112">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="0dfc4-113">このログインの使用が許可されているアプリ識別子のリスト。</span><span class="sxs-lookup"><span data-stu-id="0dfc4-113">List of app identifiers that are allowed to use this login.</span></span> <span data-ttu-id="0dfc4-114">このフィールドを省略した場合、ログインはデバイス上のすべてのアプリケーションに適用されます。</span><span class="sxs-lookup"><span data-stu-id="0dfc4-114">If this field is omitted, the login applies to all applications on the device.</span></span> <span data-ttu-id="0dfc4-115">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="0dfc4-115">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="0dfc4-116">allowedUrls</span><span class="sxs-lookup"><span data-stu-id="0dfc4-116">allowedUrls</span></span>|<span data-ttu-id="0dfc4-117">String collection</span><span class="sxs-lookup"><span data-stu-id="0dfc4-117">String collection</span></span>|<span data-ttu-id="0dfc4-118">このログインを使用するために一致する必要がある HTTP Url のリスト。</span><span class="sxs-lookup"><span data-stu-id="0dfc4-118">List of HTTP URLs that must be matched in order to use this login.</span></span> <span data-ttu-id="0dfc4-119">IOS 9.0 以降では、ワイルドカード文字を使用することができます。</span><span class="sxs-lookup"><span data-stu-id="0dfc4-119">With iOS 9.0 or later, a wildcard characters may be used.</span></span>|
|<span data-ttu-id="0dfc4-120">displayName</span><span class="sxs-lookup"><span data-stu-id="0dfc4-120">displayName</span></span>|<span data-ttu-id="0dfc4-121">String</span><span class="sxs-lookup"><span data-stu-id="0dfc4-121">String</span></span>|<span data-ttu-id="0dfc4-122">受信側デバイスに表示されるログイン設定の表示名。</span><span class="sxs-lookup"><span data-stu-id="0dfc4-122">The display name of login settings shown on the receiving device.</span></span>|
|<span data-ttu-id="0dfc4-123">kerberosPrincipalName</span><span class="sxs-lookup"><span data-stu-id="0dfc4-123">kerberosPrincipalName</span></span>|<span data-ttu-id="0dfc4-124">String</span><span class="sxs-lookup"><span data-stu-id="0dfc4-124">String</span></span>|<span data-ttu-id="0dfc4-125">Kerberos プリンシパル名。</span><span class="sxs-lookup"><span data-stu-id="0dfc4-125">A Kerberos principal name.</span></span> <span data-ttu-id="0dfc4-126">指定しない場合、プロファイルのインストール時にユーザーに対してプロンプトが表示されます。</span><span class="sxs-lookup"><span data-stu-id="0dfc4-126">If not provided, the user is prompted for one during profile installation.</span></span>|
|<span data-ttu-id="0dfc4-127">kerberosRealm</span><span class="sxs-lookup"><span data-stu-id="0dfc4-127">kerberosRealm</span></span>|<span data-ttu-id="0dfc4-128">String</span><span class="sxs-lookup"><span data-stu-id="0dfc4-128">String</span></span>|<span data-ttu-id="0dfc4-129">Kerberos 領域名。</span><span class="sxs-lookup"><span data-stu-id="0dfc4-129">A Kerberos realm name.</span></span> <span data-ttu-id="0dfc4-130">大文字小文字を区別します。</span><span class="sxs-lookup"><span data-stu-id="0dfc4-130">Case sensitive.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0dfc4-131">関係</span><span class="sxs-lookup"><span data-stu-id="0dfc4-131">Relationships</span></span>
<span data-ttu-id="0dfc4-132">なし</span><span class="sxs-lookup"><span data-stu-id="0dfc4-132">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0dfc4-133">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="0dfc4-133">JSON Representation</span></span>
<span data-ttu-id="0dfc4-134">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="0dfc4-134">Here is a JSON representation of the resource.</span></span>
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




