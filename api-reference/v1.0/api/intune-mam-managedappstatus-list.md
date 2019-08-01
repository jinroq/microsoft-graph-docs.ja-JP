---
title: managedAppStatuses のリスト
description: managedAppStatus オブジェクトのプロパティとリレーションシップをリストします。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 32911404b7faba66239e87bca8c1cfc766758920
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35996659"
---
# <a name="list-managedappstatuses"></a><span data-ttu-id="f51f7-103">managedAppStatuses のリスト</span><span class="sxs-lookup"><span data-stu-id="f51f7-103">List managedAppStatuses</span></span>

> <span data-ttu-id="f51f7-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="f51f7-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f51f7-105">[managedAppStatus](../resources/intune-mam-managedappstatus.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="f51f7-105">List properties and relationships of the [managedAppStatus](../resources/intune-mam-managedappstatus.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f51f7-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="f51f7-106">Prerequisites</span></span>
<span data-ttu-id="f51f7-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f51f7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f51f7-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f51f7-109">Permission type</span></span>|<span data-ttu-id="f51f7-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="f51f7-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f51f7-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f51f7-111">Delegated (work or school account)</span></span>|<span data-ttu-id="f51f7-112">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="f51f7-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="f51f7-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f51f7-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f51f7-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f51f7-114">Not supported.</span></span>|
|<span data-ttu-id="f51f7-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f51f7-115">Application</span></span>|<span data-ttu-id="f51f7-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f51f7-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f51f7-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f51f7-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppStatuses
```

## <a name="request-headers"></a><span data-ttu-id="f51f7-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f51f7-118">Request headers</span></span>
|<span data-ttu-id="f51f7-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f51f7-119">Header</span></span>|<span data-ttu-id="f51f7-120">値</span><span class="sxs-lookup"><span data-stu-id="f51f7-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f51f7-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="f51f7-121">Authorization</span></span>|<span data-ttu-id="f51f7-122">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="f51f7-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f51f7-123">承諾</span><span class="sxs-lookup"><span data-stu-id="f51f7-123">Accept</span></span>|<span data-ttu-id="f51f7-124">application/json</span><span class="sxs-lookup"><span data-stu-id="f51f7-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f51f7-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="f51f7-125">Request body</span></span>
<span data-ttu-id="f51f7-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="f51f7-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f51f7-127">応答</span><span class="sxs-lookup"><span data-stu-id="f51f7-127">Response</span></span>
<span data-ttu-id="f51f7-128">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [managedAppStatus](../resources/intune-mam-managedappstatus.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="f51f7-128">If successful, this method returns a `200 OK` response code and a collection of [managedAppStatus](../resources/intune-mam-managedappstatus.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f51f7-129">例</span><span class="sxs-lookup"><span data-stu-id="f51f7-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="f51f7-130">要求</span><span class="sxs-lookup"><span data-stu-id="f51f7-130">Request</span></span>
<span data-ttu-id="f51f7-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="f51f7-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedAppStatuses
```

### <a name="response"></a><span data-ttu-id="f51f7-132">応答</span><span class="sxs-lookup"><span data-stu-id="f51f7-132">Response</span></span>
<span data-ttu-id="f51f7-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="f51f7-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 227

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managedAppStatus",
      "displayName": "Display Name value",
      "id": "ad1f7541-7541-ad1f-4175-1fad41751fad",
      "version": "Version value"
    }
  ]
}
```



