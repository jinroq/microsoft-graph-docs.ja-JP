---
title: setMobileDeviceManagementAuthority アクション
description: モバイル デバイス管理権限の設定
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 687c35463f4ebaffb7571cd8bd48ca50b5c213c3
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36352442"
---
# <a name="setmobiledevicemanagementauthority-action"></a><span data-ttu-id="3c953-103">setMobileDeviceManagementAuthority アクション</span><span class="sxs-lookup"><span data-stu-id="3c953-103">setMobileDeviceManagementAuthority action</span></span>

> <span data-ttu-id="3c953-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3c953-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3c953-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="3c953-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3c953-106">モバイル デバイス管理権限の設定</span><span class="sxs-lookup"><span data-stu-id="3c953-106">Set mobile device management authority</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3c953-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="3c953-107">Prerequisites</span></span>
<span data-ttu-id="3c953-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3c953-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3c953-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="3c953-110">Permission type</span></span>|<span data-ttu-id="3c953-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="3c953-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3c953-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="3c953-112">Delegated (work or school account)</span></span>|<span data-ttu-id="3c953-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3c953-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="3c953-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="3c953-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3c953-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3c953-115">Not supported.</span></span>|
|<span data-ttu-id="3c953-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="3c953-116">Application</span></span>|<span data-ttu-id="3c953-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3c953-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3c953-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="3c953-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /organization/{organizationId}/setMobileDeviceManagementAuthority
```

## <a name="request-headers"></a><span data-ttu-id="3c953-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3c953-119">Request headers</span></span>
|<span data-ttu-id="3c953-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3c953-120">Header</span></span>|<span data-ttu-id="3c953-121">値</span><span class="sxs-lookup"><span data-stu-id="3c953-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3c953-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="3c953-122">Authorization</span></span>|<span data-ttu-id="3c953-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="3c953-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3c953-124">承諾</span><span class="sxs-lookup"><span data-stu-id="3c953-124">Accept</span></span>|<span data-ttu-id="3c953-125">application/json</span><span class="sxs-lookup"><span data-stu-id="3c953-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3c953-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="3c953-126">Request body</span></span>
<span data-ttu-id="3c953-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="3c953-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3c953-128">応答</span><span class="sxs-lookup"><span data-stu-id="3c953-128">Response</span></span>
<span data-ttu-id="3c953-129">成功した場合、この関数は `200 OK` 応答コードと、応答本文で Int32 を返します。</span><span class="sxs-lookup"><span data-stu-id="3c953-129">If successful, this action returns a `200 OK` response code and a Int32 in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3c953-130">例</span><span class="sxs-lookup"><span data-stu-id="3c953-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="3c953-131">要求</span><span class="sxs-lookup"><span data-stu-id="3c953-131">Request</span></span>
<span data-ttu-id="3c953-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="3c953-132">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/organization/{organizationId}/setMobileDeviceManagementAuthority
```

### <a name="response"></a><span data-ttu-id="3c953-133">応答</span><span class="sxs-lookup"><span data-stu-id="3c953-133">Response</span></span>
<span data-ttu-id="3c953-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="3c953-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 18

{
  "value": 2
}
```






