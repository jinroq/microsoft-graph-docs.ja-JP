---
title: officeClientConfigurationAssignment の削除
description: officeClientConfigurationAssignment を削除します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 49b4401887276957ecf220802ae67a3803497212
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30151416"
---
# <a name="delete-officeclientconfigurationassignment"></a><span data-ttu-id="3c6cc-103">officeClientConfigurationAssignment の削除</span><span class="sxs-lookup"><span data-stu-id="3c6cc-103">Delete officeClientConfigurationAssignment</span></span>

> <span data-ttu-id="3c6cc-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3c6cc-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3c6cc-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="3c6cc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3c6cc-106">[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="3c6cc-106">Deletes a [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3c6cc-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="3c6cc-107">Prerequisites</span></span>
<span data-ttu-id="3c6cc-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3c6cc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3c6cc-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="3c6cc-110">Permission type</span></span>|<span data-ttu-id="3c6cc-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="3c6cc-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3c6cc-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="3c6cc-112">Delegated (work or school account)</span></span>|<span data-ttu-id="3c6cc-113">\* \* TODO: 範囲を決定します \* \*</span><span class="sxs-lookup"><span data-stu-id="3c6cc-113">\*\*TODO: Determine scopes \*\*</span></span>|
|<span data-ttu-id="3c6cc-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="3c6cc-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3c6cc-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3c6cc-115">Not supported.</span></span>|
|<span data-ttu-id="3c6cc-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="3c6cc-116">Application</span></span>|<span data-ttu-id="3c6cc-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3c6cc-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3c6cc-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="3c6cc-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /officeConfiguration/clientConfigurations/{officeClientConfigurationId}/assignments/{officeClientConfigurationAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="3c6cc-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3c6cc-119">Request headers</span></span>
|<span data-ttu-id="3c6cc-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3c6cc-120">Header</span></span>|<span data-ttu-id="3c6cc-121">値</span><span class="sxs-lookup"><span data-stu-id="3c6cc-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3c6cc-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="3c6cc-122">Authorization</span></span>|<span data-ttu-id="3c6cc-123">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="3c6cc-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3c6cc-124">承諾</span><span class="sxs-lookup"><span data-stu-id="3c6cc-124">Accept</span></span>|<span data-ttu-id="3c6cc-125">application/json</span><span class="sxs-lookup"><span data-stu-id="3c6cc-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3c6cc-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="3c6cc-126">Request body</span></span>
<span data-ttu-id="3c6cc-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="3c6cc-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3c6cc-128">応答</span><span class="sxs-lookup"><span data-stu-id="3c6cc-128">Response</span></span>
<span data-ttu-id="3c6cc-129">成功した場合、このメソッドは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="3c6cc-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="3c6cc-130">例</span><span class="sxs-lookup"><span data-stu-id="3c6cc-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="3c6cc-131">要求</span><span class="sxs-lookup"><span data-stu-id="3c6cc-131">Request</span></span>
<span data-ttu-id="3c6cc-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="3c6cc-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/officeConfiguration/clientConfigurations/{officeClientConfigurationId}/assignments/{officeClientConfigurationAssignmentId}
```

### <a name="response"></a><span data-ttu-id="3c6cc-133">応答</span><span class="sxs-lookup"><span data-stu-id="3c6cc-133">Response</span></span>
<span data-ttu-id="3c6cc-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="3c6cc-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



