---
title: completeSignup アクション
description: まだ文書化されていません
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 3e6e71dafb3ed597213e23c717d03d0876102cae
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36322780"
---
# <a name="completesignup-action"></a><span data-ttu-id="dae07-103">completeSignup アクション</span><span class="sxs-lookup"><span data-stu-id="dae07-103">completeSignup action</span></span>

> <span data-ttu-id="dae07-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="dae07-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dae07-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="dae07-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dae07-106">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="dae07-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="dae07-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="dae07-107">Prerequisites</span></span>
<span data-ttu-id="dae07-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="dae07-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dae07-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="dae07-110">Permission type</span></span>|<span data-ttu-id="dae07-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="dae07-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dae07-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="dae07-112">Delegated (work or school account)</span></span>|<span data-ttu-id="dae07-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dae07-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="dae07-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="dae07-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dae07-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="dae07-115">Not supported.</span></span>|
|<span data-ttu-id="dae07-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="dae07-116">Application</span></span>|<span data-ttu-id="dae07-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dae07-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="dae07-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="dae07-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/androidManagedStoreAccountEnterpriseSettings/completeSignup
```

## <a name="request-headers"></a><span data-ttu-id="dae07-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="dae07-119">Request headers</span></span>
|<span data-ttu-id="dae07-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="dae07-120">Header</span></span>|<span data-ttu-id="dae07-121">値</span><span class="sxs-lookup"><span data-stu-id="dae07-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dae07-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="dae07-122">Authorization</span></span>|<span data-ttu-id="dae07-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="dae07-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dae07-124">承諾</span><span class="sxs-lookup"><span data-stu-id="dae07-124">Accept</span></span>|<span data-ttu-id="dae07-125">application/json</span><span class="sxs-lookup"><span data-stu-id="dae07-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dae07-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="dae07-126">Request body</span></span>
<span data-ttu-id="dae07-127">要求本文で、パラメーターの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="dae07-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="dae07-128">次の表に、このアクションで使用できるパラメーターを示します。</span><span class="sxs-lookup"><span data-stu-id="dae07-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="dae07-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="dae07-129">Property</span></span>|<span data-ttu-id="dae07-130">型</span><span class="sxs-lookup"><span data-stu-id="dae07-130">Type</span></span>|<span data-ttu-id="dae07-131">説明</span><span class="sxs-lookup"><span data-stu-id="dae07-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dae07-132">enterpriseToken</span><span class="sxs-lookup"><span data-stu-id="dae07-132">enterpriseToken</span></span>|<span data-ttu-id="dae07-133">String</span><span class="sxs-lookup"><span data-stu-id="dae07-133">String</span></span>|<span data-ttu-id="dae07-134">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="dae07-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="dae07-135">応答</span><span class="sxs-lookup"><span data-stu-id="dae07-135">Response</span></span>
<span data-ttu-id="dae07-136">成功した場合、このアクションは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="dae07-136">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="dae07-137">例</span><span class="sxs-lookup"><span data-stu-id="dae07-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="dae07-138">要求</span><span class="sxs-lookup"><span data-stu-id="dae07-138">Request</span></span>
<span data-ttu-id="dae07-139">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="dae07-139">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/androidManagedStoreAccountEnterpriseSettings/completeSignup

Content-type: application/json
Content-length: 51

{
  "enterpriseToken": "Enterprise Token value"
}
```

### <a name="response"></a><span data-ttu-id="dae07-140">応答</span><span class="sxs-lookup"><span data-stu-id="dae07-140">Response</span></span>
<span data-ttu-id="dae07-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="dae07-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```






