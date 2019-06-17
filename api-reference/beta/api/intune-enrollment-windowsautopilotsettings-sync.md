---
title: sync アクション
description: まだ文書化されていません
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 63c7e876db560514edc7550dd72bee47b411333e
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34982715"
---
# <a name="sync-action"></a><span data-ttu-id="fda4e-103">同期アクション</span><span class="sxs-lookup"><span data-stu-id="fda4e-103">sync action</span></span>

> <span data-ttu-id="fda4e-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fda4e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fda4e-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="fda4e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fda4e-106">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="fda4e-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fda4e-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="fda4e-107">Prerequisites</span></span>
<span data-ttu-id="fda4e-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="fda4e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fda4e-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="fda4e-110">Permission type</span></span>|<span data-ttu-id="fda4e-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="fda4e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fda4e-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="fda4e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="fda4e-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fda4e-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="fda4e-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="fda4e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fda4e-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fda4e-115">Not supported.</span></span>|
|<span data-ttu-id="fda4e-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="fda4e-116">Application</span></span>|<span data-ttu-id="fda4e-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fda4e-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fda4e-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="fda4e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsAutopilotSettings/sync
```

## <a name="request-headers"></a><span data-ttu-id="fda4e-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="fda4e-119">Request headers</span></span>
|<span data-ttu-id="fda4e-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="fda4e-120">Header</span></span>|<span data-ttu-id="fda4e-121">値</span><span class="sxs-lookup"><span data-stu-id="fda4e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fda4e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="fda4e-122">Authorization</span></span>|<span data-ttu-id="fda4e-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="fda4e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fda4e-124">承諾</span><span class="sxs-lookup"><span data-stu-id="fda4e-124">Accept</span></span>|<span data-ttu-id="fda4e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="fda4e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fda4e-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="fda4e-126">Request body</span></span>
<span data-ttu-id="fda4e-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="fda4e-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fda4e-128">応答</span><span class="sxs-lookup"><span data-stu-id="fda4e-128">Response</span></span>
<span data-ttu-id="fda4e-129">成功した場合、このアクションは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="fda4e-129">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="fda4e-130">例</span><span class="sxs-lookup"><span data-stu-id="fda4e-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="fda4e-131">要求</span><span class="sxs-lookup"><span data-stu-id="fda4e-131">Request</span></span>
<span data-ttu-id="fda4e-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="fda4e-132">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotSettings/sync
```

### <a name="response"></a><span data-ttu-id="fda4e-133">応答</span><span class="sxs-lookup"><span data-stu-id="fda4e-133">Response</span></span>
<span data-ttu-id="fda4e-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="fda4e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





