---
title: enableLegacyPcManagement アクション
description: まだ文書化されていません
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: ca77a6aed291f9a4e8c201437d43a4cfc0bde1c5
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30153873"
---
# <a name="enablelegacypcmanagement-action"></a><span data-ttu-id="a7dde-103">enableLegacyPcManagement アクション</span><span class="sxs-lookup"><span data-stu-id="a7dde-103">enableLegacyPcManagement action</span></span>

> <span data-ttu-id="a7dde-104">**重要:** Microsoft Graph の/ベータ版の api は変更される可能性があります。</span><span class="sxs-lookup"><span data-stu-id="a7dde-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="a7dde-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a7dde-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a7dde-106">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="a7dde-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a7dde-107">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="a7dde-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a7dde-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="a7dde-108">Prerequisites</span></span>
<span data-ttu-id="a7dde-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a7dde-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference).</span></span>

|<span data-ttu-id="a7dde-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a7dde-111">Permission type</span></span>|<span data-ttu-id="a7dde-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="a7dde-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a7dde-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a7dde-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="a7dde-114">&nbsp; &nbsp; **デバイス構成**</span><span class="sxs-lookup"><span data-stu-id="a7dde-114">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="a7dde-115">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a7dde-115">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a7dde-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a7dde-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a7dde-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a7dde-117">Not supported.</span></span>|
|<span data-ttu-id="a7dde-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a7dde-118">Application</span></span>|<span data-ttu-id="a7dde-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a7dde-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a7dde-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a7dde-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/enableLegacyPcManagement
```

## <a name="request-headers"></a><span data-ttu-id="a7dde-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a7dde-121">Request headers</span></span>
|<span data-ttu-id="a7dde-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a7dde-122">Header</span></span>|<span data-ttu-id="a7dde-123">値</span><span class="sxs-lookup"><span data-stu-id="a7dde-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a7dde-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="a7dde-124">Authorization</span></span>|<span data-ttu-id="a7dde-125">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="a7dde-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a7dde-126">承諾</span><span class="sxs-lookup"><span data-stu-id="a7dde-126">Accept</span></span>|<span data-ttu-id="a7dde-127">application/json</span><span class="sxs-lookup"><span data-stu-id="a7dde-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a7dde-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="a7dde-128">Request body</span></span>
<span data-ttu-id="a7dde-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="a7dde-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a7dde-130">応答</span><span class="sxs-lookup"><span data-stu-id="a7dde-130">Response</span></span>
<span data-ttu-id="a7dde-131">成功した場合、このアクションは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="a7dde-131">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="a7dde-132">例</span><span class="sxs-lookup"><span data-stu-id="a7dde-132">Example</span></span>
### <a name="request"></a><span data-ttu-id="a7dde-133">要求</span><span class="sxs-lookup"><span data-stu-id="a7dde-133">Request</span></span>
<span data-ttu-id="a7dde-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="a7dde-134">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/enableLegacyPcManagement
```

### <a name="response"></a><span data-ttu-id="a7dde-135">応答</span><span class="sxs-lookup"><span data-stu-id="a7dde-135">Response</span></span>
<span data-ttu-id="a7dde-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="a7dde-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





