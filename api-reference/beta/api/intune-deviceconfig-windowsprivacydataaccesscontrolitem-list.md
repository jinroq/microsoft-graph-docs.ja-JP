---
title: リスト windowsPrivacyDataAccessControlItems
description: WindowsPrivacyDataAccessControlItem オブジェクトのプロパティとリレーションシップをリストします。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7189885a84703315500a4ce4fc14a2367b4b31b5
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33917444"
---
# <a name="list-windowsprivacydataaccesscontrolitems"></a><span data-ttu-id="bb581-103">リスト windowsPrivacyDataAccessControlItems</span><span class="sxs-lookup"><span data-stu-id="bb581-103">List windowsPrivacyDataAccessControlItems</span></span>

> <span data-ttu-id="bb581-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bb581-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bb581-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="bb581-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bb581-106">[WindowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="bb581-106">List properties and relationships of the [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bb581-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="bb581-107">Prerequisites</span></span>
<span data-ttu-id="bb581-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="bb581-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bb581-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="bb581-110">Permission type</span></span>|<span data-ttu-id="bb581-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="bb581-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bb581-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="bb581-112">Delegated (work or school account)</span></span>|<span data-ttu-id="bb581-113">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="bb581-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="bb581-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="bb581-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bb581-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bb581-115">Not supported.</span></span>|
|<span data-ttu-id="bb581-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="bb581-116">Application</span></span>|<span data-ttu-id="bb581-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bb581-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bb581-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="bb581-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windows10GeneralConfiguration/privacyAccessControls
```

## <a name="request-headers"></a><span data-ttu-id="bb581-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="bb581-119">Request headers</span></span>
|<span data-ttu-id="bb581-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="bb581-120">Header</span></span>|<span data-ttu-id="bb581-121">値</span><span class="sxs-lookup"><span data-stu-id="bb581-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bb581-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="bb581-122">Authorization</span></span>|<span data-ttu-id="bb581-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="bb581-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bb581-124">承諾</span><span class="sxs-lookup"><span data-stu-id="bb581-124">Accept</span></span>|<span data-ttu-id="bb581-125">application/json</span><span class="sxs-lookup"><span data-stu-id="bb581-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bb581-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="bb581-126">Request body</span></span>
<span data-ttu-id="bb581-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="bb581-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bb581-128">応答</span><span class="sxs-lookup"><span data-stu-id="bb581-128">Response</span></span>
<span data-ttu-id="bb581-129">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="bb581-129">If successful, this method returns a `200 OK` response code and a collection of [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bb581-130">例</span><span class="sxs-lookup"><span data-stu-id="bb581-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="bb581-131">要求</span><span class="sxs-lookup"><span data-stu-id="bb581-131">Request</span></span>
<span data-ttu-id="bb581-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="bb581-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windows10GeneralConfiguration/privacyAccessControls
```

### <a name="response"></a><span data-ttu-id="bb581-133">応答</span><span class="sxs-lookup"><span data-stu-id="bb581-133">Response</span></span>
<span data-ttu-id="bb581-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="bb581-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 356

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsPrivacyDataAccessControlItem",
      "id": "03b15556-5556-03b1-5655-b1035655b103",
      "accessLevel": "forceAllow",
      "dataCategory": "accountInfo",
      "appPackageFamilyName": "App Package Family Name value",
      "appDisplayName": "App Display Name value"
    }
  ]
}
```




