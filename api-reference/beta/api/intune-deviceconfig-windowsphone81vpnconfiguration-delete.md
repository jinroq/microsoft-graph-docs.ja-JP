---
title: WindowsPhone81VpnConfiguration の削除
description: WindowsPhone81VpnConfiguration を削除します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: ad7318bed7737ae0077a36604d54106bf622faef
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36338330"
---
# <a name="delete-windowsphone81vpnconfiguration"></a><span data-ttu-id="f65ac-103">WindowsPhone81VpnConfiguration の削除</span><span class="sxs-lookup"><span data-stu-id="f65ac-103">Delete windowsPhone81VpnConfiguration</span></span>

> <span data-ttu-id="f65ac-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f65ac-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f65ac-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="f65ac-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f65ac-106">[WindowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="f65ac-106">Deletes a [windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f65ac-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="f65ac-107">Prerequisites</span></span>
<span data-ttu-id="f65ac-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f65ac-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f65ac-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f65ac-110">Permission type</span></span>|<span data-ttu-id="f65ac-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="f65ac-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f65ac-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f65ac-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f65ac-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f65ac-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f65ac-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f65ac-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f65ac-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f65ac-115">Not supported.</span></span>|
|<span data-ttu-id="f65ac-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f65ac-116">Application</span></span>|<span data-ttu-id="f65ac-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f65ac-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f65ac-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f65ac-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="f65ac-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f65ac-119">Request headers</span></span>
|<span data-ttu-id="f65ac-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f65ac-120">Header</span></span>|<span data-ttu-id="f65ac-121">値</span><span class="sxs-lookup"><span data-stu-id="f65ac-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f65ac-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f65ac-122">Authorization</span></span>|<span data-ttu-id="f65ac-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="f65ac-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f65ac-124">承諾</span><span class="sxs-lookup"><span data-stu-id="f65ac-124">Accept</span></span>|<span data-ttu-id="f65ac-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f65ac-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f65ac-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="f65ac-126">Request body</span></span>
<span data-ttu-id="f65ac-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="f65ac-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f65ac-128">応答</span><span class="sxs-lookup"><span data-stu-id="f65ac-128">Response</span></span>
<span data-ttu-id="f65ac-129">成功した場合、このメソッドは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="f65ac-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="f65ac-130">例</span><span class="sxs-lookup"><span data-stu-id="f65ac-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="f65ac-131">要求</span><span class="sxs-lookup"><span data-stu-id="f65ac-131">Request</span></span>
<span data-ttu-id="f65ac-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="f65ac-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="f65ac-133">応答</span><span class="sxs-lookup"><span data-stu-id="f65ac-133">Response</span></span>
<span data-ttu-id="f65ac-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="f65ac-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```






