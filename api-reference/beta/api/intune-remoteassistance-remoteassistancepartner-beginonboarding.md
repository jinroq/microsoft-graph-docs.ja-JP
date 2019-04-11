---
title: beginOnboarding アクション
description: オンボードを開始する要求。  適切な TeamViewer アカウント情報と組み合わせる必要があります。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 36fa3b2d27bbcad94ad2427c5a248a3ae5360fc8
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31789872"
---
# <a name="beginonboarding-action"></a><span data-ttu-id="2d07f-104">beginOnboarding アクション</span><span class="sxs-lookup"><span data-stu-id="2d07f-104">beginOnboarding action</span></span>

> <span data-ttu-id="2d07f-105">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2d07f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2d07f-106">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="2d07f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2d07f-107">オンボードを開始する要求。</span><span class="sxs-lookup"><span data-stu-id="2d07f-107">A request to start onboarding.</span></span>  <span data-ttu-id="2d07f-108">適切な TeamViewer アカウント情報と組み合わせる必要があります。</span><span class="sxs-lookup"><span data-stu-id="2d07f-108">Must be coupled with the appropriate TeamViewer account information</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2d07f-109">前提条件</span><span class="sxs-lookup"><span data-stu-id="2d07f-109">Prerequisites</span></span>
<span data-ttu-id="2d07f-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2d07f-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2d07f-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="2d07f-112">Permission type</span></span>|<span data-ttu-id="2d07f-113">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="2d07f-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2d07f-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="2d07f-114">Delegated (work or school account)</span></span>|<span data-ttu-id="2d07f-115">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2d07f-115">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="2d07f-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="2d07f-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2d07f-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2d07f-117">Not supported.</span></span>|
|<span data-ttu-id="2d07f-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="2d07f-118">Application</span></span>|<span data-ttu-id="2d07f-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2d07f-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2d07f-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="2d07f-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/remoteAssistancePartners/{remoteAssistancePartnerId}/beginOnboarding
```

## <a name="request-headers"></a><span data-ttu-id="2d07f-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2d07f-121">Request headers</span></span>
|<span data-ttu-id="2d07f-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2d07f-122">Header</span></span>|<span data-ttu-id="2d07f-123">値</span><span class="sxs-lookup"><span data-stu-id="2d07f-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2d07f-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="2d07f-124">Authorization</span></span>|<span data-ttu-id="2d07f-125">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="2d07f-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2d07f-126">承諾</span><span class="sxs-lookup"><span data-stu-id="2d07f-126">Accept</span></span>|<span data-ttu-id="2d07f-127">application/json</span><span class="sxs-lookup"><span data-stu-id="2d07f-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2d07f-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="2d07f-128">Request body</span></span>
<span data-ttu-id="2d07f-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="2d07f-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2d07f-130">応答</span><span class="sxs-lookup"><span data-stu-id="2d07f-130">Response</span></span>
<span data-ttu-id="2d07f-131">成功した場合、このアクションは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="2d07f-131">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="2d07f-132">例</span><span class="sxs-lookup"><span data-stu-id="2d07f-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="2d07f-133">要求</span><span class="sxs-lookup"><span data-stu-id="2d07f-133">Request</span></span>
<span data-ttu-id="2d07f-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="2d07f-134">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/remoteAssistancePartners/{remoteAssistancePartnerId}/beginOnboarding
```

### <a name="response"></a><span data-ttu-id="2d07f-135">応答</span><span class="sxs-lookup"><span data-stu-id="2d07f-135">Response</span></span>
<span data-ttu-id="2d07f-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="2d07f-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





