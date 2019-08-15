---
title: OfficeClientConfigurationAssignment の削除
description: OfficeClientConfigurationAssignment を削除します。
localization_priority: Normal
author: rolyon
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b44c6da84696cc4bafdbcbdb2ddf15d970399bfd
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/15/2019
ms.locfileid: "36420841"
---
# <a name="delete-officeclientconfigurationassignment"></a><span data-ttu-id="52500-103">OfficeClientConfigurationAssignment の削除</span><span class="sxs-lookup"><span data-stu-id="52500-103">Delete officeClientConfigurationAssignment</span></span>

> <span data-ttu-id="52500-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="52500-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="52500-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="52500-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="52500-106">[OfficeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="52500-106">Deletes a [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="52500-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="52500-107">Prerequisites</span></span>
<span data-ttu-id="52500-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="52500-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="52500-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="52500-110">Permission type</span></span>|<span data-ttu-id="52500-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="52500-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="52500-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="52500-112">Delegated (work or school account)</span></span>|<span data-ttu-id="52500-113">**TODO: スコープを決定する**</span><span class="sxs-lookup"><span data-stu-id="52500-113">**TODO: Determine scopes**</span></span>|
|<span data-ttu-id="52500-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="52500-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="52500-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="52500-115">Not supported.</span></span>|
|<span data-ttu-id="52500-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="52500-116">Application</span></span>|<span data-ttu-id="52500-117">\* \* TODO: 範囲を決定します \* \*</span><span class="sxs-lookup"><span data-stu-id="52500-117">\*\*TODO: Determine scopes \*\*</span></span>|

## <a name="http-request"></a><span data-ttu-id="52500-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="52500-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /officeConfiguration/clientConfigurations/{officeClientConfigurationId}/assignments/{officeClientConfigurationAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="52500-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="52500-119">Request headers</span></span>
|<span data-ttu-id="52500-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="52500-120">Header</span></span>|<span data-ttu-id="52500-121">値</span><span class="sxs-lookup"><span data-stu-id="52500-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="52500-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="52500-122">Authorization</span></span>|<span data-ttu-id="52500-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="52500-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="52500-124">承諾</span><span class="sxs-lookup"><span data-stu-id="52500-124">Accept</span></span>|<span data-ttu-id="52500-125">application/json</span><span class="sxs-lookup"><span data-stu-id="52500-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="52500-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="52500-126">Request body</span></span>
<span data-ttu-id="52500-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="52500-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="52500-128">応答</span><span class="sxs-lookup"><span data-stu-id="52500-128">Response</span></span>
<span data-ttu-id="52500-129">成功した場合、このメソッドは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="52500-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="52500-130">例</span><span class="sxs-lookup"><span data-stu-id="52500-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="52500-131">要求</span><span class="sxs-lookup"><span data-stu-id="52500-131">Request</span></span>
<span data-ttu-id="52500-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="52500-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/officeConfiguration/clientConfigurations/{officeClientConfigurationId}/assignments/{officeClientConfigurationAssignmentId}
```

### <a name="response"></a><span data-ttu-id="52500-133">応答</span><span class="sxs-lookup"><span data-stu-id="52500-133">Response</span></span>
<span data-ttu-id="52500-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="52500-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```






