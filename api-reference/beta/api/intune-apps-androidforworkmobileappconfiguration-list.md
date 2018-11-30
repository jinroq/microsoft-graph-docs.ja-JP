---
title: リスト androidForWorkMobileAppConfigurations
description: AndroidForWorkMobileAppConfiguration オブジェクトのプロパティと関係を一覧表示します。
ms.openlocfilehash: 3afc99521fc9dcc9118c3c619a1bf8ef619cc040
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27067368"
---
# <a name="list-androidforworkmobileappconfigurations"></a><span data-ttu-id="36cab-103">リスト androidForWorkMobileAppConfigurations</span><span class="sxs-lookup"><span data-stu-id="36cab-103">List androidForWorkMobileAppConfigurations</span></span>

> <span data-ttu-id="36cab-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="36cab-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="36cab-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="36cab-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="36cab-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="36cab-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="36cab-107">[AndroidForWorkMobileAppConfiguration](../resources/intune-apps-androidforworkmobileappconfiguration.md)オブジェクトのプロパティと関係を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="36cab-107">List properties and relationships of the [androidForWorkMobileAppConfiguration](../resources/intune-apps-androidforworkmobileappconfiguration.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="36cab-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="36cab-108">Prerequisites</span></span>
<span data-ttu-id="36cab-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="36cab-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="36cab-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="36cab-111">Permission type</span></span>|<span data-ttu-id="36cab-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="36cab-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="36cab-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="36cab-113">Delegated (work or school account)</span></span>|<span data-ttu-id="36cab-114">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="36cab-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="36cab-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="36cab-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="36cab-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="36cab-116">Not supported.</span></span>|
|<span data-ttu-id="36cab-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="36cab-117">Application</span></span>|<span data-ttu-id="36cab-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="36cab-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="36cab-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="36cab-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileAppConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="36cab-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="36cab-120">Request headers</span></span>
|<span data-ttu-id="36cab-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="36cab-121">Header</span></span>|<span data-ttu-id="36cab-122">値</span><span class="sxs-lookup"><span data-stu-id="36cab-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="36cab-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="36cab-123">Authorization</span></span>|<span data-ttu-id="36cab-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="36cab-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="36cab-125">Accept</span><span class="sxs-lookup"><span data-stu-id="36cab-125">Accept</span></span>|<span data-ttu-id="36cab-126">application/json</span><span class="sxs-lookup"><span data-stu-id="36cab-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="36cab-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="36cab-127">Request body</span></span>
<span data-ttu-id="36cab-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="36cab-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="36cab-129">応答</span><span class="sxs-lookup"><span data-stu-id="36cab-129">Response</span></span>
<span data-ttu-id="36cab-130">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に[androidForWorkMobileAppConfiguration](../resources/intune-apps-androidforworkmobileappconfiguration.md)オブジェクトのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="36cab-130">If successful, this method returns a `200 OK` response code and a collection of [androidForWorkMobileAppConfiguration](../resources/intune-apps-androidforworkmobileappconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="36cab-131">例</span><span class="sxs-lookup"><span data-stu-id="36cab-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="36cab-132">要求</span><span class="sxs-lookup"><span data-stu-id="36cab-132">Request</span></span>
<span data-ttu-id="36cab-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="36cab-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations
```

### <a name="response"></a><span data-ttu-id="36cab-134">応答</span><span class="sxs-lookup"><span data-stu-id="36cab-134">Response</span></span>
<span data-ttu-id="36cab-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="36cab-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 853

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.androidForWorkMobileAppConfiguration",
      "id": "6204ae6d-ae6d-6204-6dae-04626dae0462",
      "targetedMobileApps": [
        "Targeted Mobile Apps value"
      ],
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "displayName": "Display Name value",
      "version": 7,
      "packageId": "Package Id value",
      "payloadJson": "Payload Json value",
      "permissionActions": [
        {
          "@odata.type": "microsoft.graph.androidPermissionAction",
          "permission": "Permission value",
          "action": "autoGrant"
        }
      ]
    }
  ]
}
```





