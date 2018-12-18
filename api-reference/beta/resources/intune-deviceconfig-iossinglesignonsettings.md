---
title: iosSingleSignOnSettings リソースの種類
description: iOS は単一のサインオンでの Kerberos 認証の設定
author: tfitzmac
ms.openlocfilehash: 6bde13865c1d6b34c433a92005681b247b99d984
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27347370"
---
# <a name="iossinglesignonsettings-resource-type"></a><span data-ttu-id="5b0ef-103">iosSingleSignOnSettings リソースの種類</span><span class="sxs-lookup"><span data-stu-id="5b0ef-103">iosSingleSignOnSettings resource type</span></span>

> <span data-ttu-id="5b0ef-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="5b0ef-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5b0ef-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5b0ef-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5b0ef-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="5b0ef-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5b0ef-107">iOS は単一のサインオンでの Kerberos 認証の設定</span><span class="sxs-lookup"><span data-stu-id="5b0ef-107">iOS Kerberos authentication settings for single sign-on</span></span>
## <a name="properties"></a><span data-ttu-id="5b0ef-108">Properties</span><span class="sxs-lookup"><span data-stu-id="5b0ef-108">Properties</span></span>
|<span data-ttu-id="5b0ef-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5b0ef-109">Property</span></span>|<span data-ttu-id="5b0ef-110">種類</span><span class="sxs-lookup"><span data-stu-id="5b0ef-110">Type</span></span>|<span data-ttu-id="5b0ef-111">説明</span><span class="sxs-lookup"><span data-stu-id="5b0ef-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5b0ef-112">allowedAppsList</span><span class="sxs-lookup"><span data-stu-id="5b0ef-112">allowedAppsList</span></span>|<span data-ttu-id="5b0ef-113">[appListItem](../resources/intune-deviceconfig-applistitem.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="5b0ef-113">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="5b0ef-114">このログインを使用するのには許可されているアプリケーションの識別子の一覧です。</span><span class="sxs-lookup"><span data-stu-id="5b0ef-114">List of app identifiers that are allowed to use this login.</span></span> <span data-ttu-id="5b0ef-115">このフィールドを省略すると、ログインは、デバイス上のすべてのアプリケーションに適用されます。</span><span class="sxs-lookup"><span data-stu-id="5b0ef-115">If this field is omitted, the login applies to all applications on the device.</span></span> <span data-ttu-id="5b0ef-116">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="5b0ef-116">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="5b0ef-117">allowedUrls</span><span class="sxs-lookup"><span data-stu-id="5b0ef-117">allowedUrls</span></span>|<span data-ttu-id="5b0ef-118">String コレクション</span><span class="sxs-lookup"><span data-stu-id="5b0ef-118">String collection</span></span>|<span data-ttu-id="5b0ef-119">このログインを使用するために一致する必要がある HTTP Url の一覧です。</span><span class="sxs-lookup"><span data-stu-id="5b0ef-119">List of HTTP URLs that must be matched in order to use this login.</span></span> <span data-ttu-id="5b0ef-120">9.0 以降、iOS でワイルドカード文字を使用することがあります。</span><span class="sxs-lookup"><span data-stu-id="5b0ef-120">With iOS 9.0 or later, a wildcard characters may be used.</span></span>|
|<span data-ttu-id="5b0ef-121">displayName</span><span class="sxs-lookup"><span data-stu-id="5b0ef-121">displayName</span></span>|<span data-ttu-id="5b0ef-122">String</span><span class="sxs-lookup"><span data-stu-id="5b0ef-122">String</span></span>|<span data-ttu-id="5b0ef-123">受信側デバイスに表示されるログインの設定の表示名。</span><span class="sxs-lookup"><span data-stu-id="5b0ef-123">The display name of login settings shown on the receiving device.</span></span>|
|<span data-ttu-id="5b0ef-124">kerberosPrincipalName</span><span class="sxs-lookup"><span data-stu-id="5b0ef-124">kerberosPrincipalName</span></span>|<span data-ttu-id="5b0ef-125">String</span><span class="sxs-lookup"><span data-stu-id="5b0ef-125">String</span></span>|<span data-ttu-id="5b0ef-126">Kerberos プリンシパルの名前です。</span><span class="sxs-lookup"><span data-stu-id="5b0ef-126">A Kerberos principal name.</span></span> <span data-ttu-id="5b0ef-127">指定しない場合、プロファイルのインストール時にいずれかの入力が求められます。</span><span class="sxs-lookup"><span data-stu-id="5b0ef-127">If not provided, the user is prompted for one during profile installation.</span></span>|
|<span data-ttu-id="5b0ef-128">kerberosRealm</span><span class="sxs-lookup"><span data-stu-id="5b0ef-128">kerberosRealm</span></span>|<span data-ttu-id="5b0ef-129">String</span><span class="sxs-lookup"><span data-stu-id="5b0ef-129">String</span></span>|<span data-ttu-id="5b0ef-130">Kerberos レルムの名前です。</span><span class="sxs-lookup"><span data-stu-id="5b0ef-130">A Kerberos realm name.</span></span> <span data-ttu-id="5b0ef-131">大文字小文字を区別します。</span><span class="sxs-lookup"><span data-stu-id="5b0ef-131">Case sensitive.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5b0ef-132">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="5b0ef-132">Relationships</span></span>
<span data-ttu-id="5b0ef-133">なし</span><span class="sxs-lookup"><span data-stu-id="5b0ef-133">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="5b0ef-134">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="5b0ef-134">JSON Representation</span></span>
<span data-ttu-id="5b0ef-135">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="5b0ef-135">Here is a JSON representation of the resource.</span></span>
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





