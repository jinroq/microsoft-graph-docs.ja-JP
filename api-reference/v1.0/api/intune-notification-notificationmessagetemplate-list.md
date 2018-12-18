---
title: notificationMessageTemplates のリスト
description: notificationMessageTemplate オブジェクトのプロパティとリレーションシップをリストします。
author: tfitzmac
ms.openlocfilehash: daf84cfc898fc62e4224826a8ae83fcf84f696b4
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27346215"
---
# <a name="list-notificationmessagetemplates"></a><span data-ttu-id="50151-103">notificationMessageTemplates のリスト</span><span class="sxs-lookup"><span data-stu-id="50151-103">List notificationMessageTemplates</span></span>

> <span data-ttu-id="50151-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="50151-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="50151-105">[notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="50151-105">List properties and relationships of the [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="50151-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="50151-106">Prerequisites</span></span>
<span data-ttu-id="50151-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="50151-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="50151-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="50151-109">Permission type</span></span>|<span data-ttu-id="50151-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="50151-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="50151-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="50151-111">Delegated (work or school account)</span></span>|<span data-ttu-id="50151-112">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="50151-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="50151-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="50151-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="50151-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="50151-114">Not supported.</span></span>|
|<span data-ttu-id="50151-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="50151-115">Application</span></span>|<span data-ttu-id="50151-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="50151-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="50151-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="50151-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/notificationMessageTemplates
```

## <a name="request-headers"></a><span data-ttu-id="50151-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="50151-118">Request headers</span></span>
|<span data-ttu-id="50151-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="50151-119">Header</span></span>|<span data-ttu-id="50151-120">値</span><span class="sxs-lookup"><span data-stu-id="50151-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="50151-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="50151-121">Authorization</span></span>|<span data-ttu-id="50151-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="50151-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="50151-123">Accept</span><span class="sxs-lookup"><span data-stu-id="50151-123">Accept</span></span>|<span data-ttu-id="50151-124">application/json</span><span class="sxs-lookup"><span data-stu-id="50151-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="50151-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="50151-125">Request body</span></span>
<span data-ttu-id="50151-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="50151-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="50151-127">応答</span><span class="sxs-lookup"><span data-stu-id="50151-127">Response</span></span>
<span data-ttu-id="50151-128">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="50151-128">If successful, this method returns a `200 OK` response code and a collection of [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="50151-129">例</span><span class="sxs-lookup"><span data-stu-id="50151-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="50151-130">要求</span><span class="sxs-lookup"><span data-stu-id="50151-130">Request</span></span>
<span data-ttu-id="50151-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="50151-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/notificationMessageTemplates
```

### <a name="response"></a><span data-ttu-id="50151-132">応答</span><span class="sxs-lookup"><span data-stu-id="50151-132">Response</span></span>
<span data-ttu-id="50151-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="50151-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 367

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.notificationMessageTemplate",
      "id": "e1db399b-399b-e1db-9b39-dbe19b39dbe1",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "displayName": "Display Name value",
      "defaultLocale": "Default Locale value",
      "brandingOptions": "includeCompanyLogo"
    }
  ]
}
```



