---
title: ManagedEBookCategory を作成します。
description: 新しい managedEBookCategory オブジェクトを作成します。
ms.openlocfilehash: 8750e8c520e3a48b2da93d05b9f701c7760b6a15
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27072855"
---
# <a name="create-managedebookcategory"></a><span data-ttu-id="60ef0-103">ManagedEBookCategory を作成します。</span><span class="sxs-lookup"><span data-stu-id="60ef0-103">Create managedEBookCategory</span></span>

> <span data-ttu-id="60ef0-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="60ef0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="60ef0-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="60ef0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="60ef0-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="60ef0-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="60ef0-107">新しい[managedEBookCategory](../resources/intune-books-managedebookcategory.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="60ef0-107">Create a new [managedEBookCategory](../resources/intune-books-managedebookcategory.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="60ef0-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="60ef0-108">Prerequisites</span></span>
<span data-ttu-id="60ef0-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="60ef0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="60ef0-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="60ef0-111">Permission type</span></span>|<span data-ttu-id="60ef0-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="60ef0-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="60ef0-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="60ef0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="60ef0-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="60ef0-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="60ef0-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="60ef0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="60ef0-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="60ef0-116">Not supported.</span></span>|
|<span data-ttu-id="60ef0-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="60ef0-117">Application</span></span>|<span data-ttu-id="60ef0-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="60ef0-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="60ef0-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="60ef0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBookCategories
POST /deviceAppManagement/managedEBooks/{managedEBookId}/categories
```

## <a name="request-headers"></a><span data-ttu-id="60ef0-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="60ef0-120">Request headers</span></span>
|<span data-ttu-id="60ef0-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="60ef0-121">Header</span></span>|<span data-ttu-id="60ef0-122">値</span><span class="sxs-lookup"><span data-stu-id="60ef0-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="60ef0-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="60ef0-123">Authorization</span></span>|<span data-ttu-id="60ef0-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="60ef0-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="60ef0-125">Accept</span><span class="sxs-lookup"><span data-stu-id="60ef0-125">Accept</span></span>|<span data-ttu-id="60ef0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="60ef0-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="60ef0-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="60ef0-127">Request body</span></span>
<span data-ttu-id="60ef0-128">要求の本文に managedEBookCategory オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="60ef0-128">In the request body, supply a JSON representation for the managedEBookCategory object.</span></span>

<span data-ttu-id="60ef0-129">次の表は、managedEBookCategory を作成するときに必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="60ef0-129">The following table shows the properties that are required when you create the managedEBookCategory.</span></span>

|<span data-ttu-id="60ef0-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="60ef0-130">Property</span></span>|<span data-ttu-id="60ef0-131">型</span><span class="sxs-lookup"><span data-stu-id="60ef0-131">Type</span></span>|<span data-ttu-id="60ef0-132">説明</span><span class="sxs-lookup"><span data-stu-id="60ef0-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="60ef0-133">id</span><span class="sxs-lookup"><span data-stu-id="60ef0-133">id</span></span>|<span data-ttu-id="60ef0-134">String</span><span class="sxs-lookup"><span data-stu-id="60ef0-134">String</span></span>|<span data-ttu-id="60ef0-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="60ef0-135">The key of the entity.</span></span>|
|<span data-ttu-id="60ef0-136">displayName</span><span class="sxs-lookup"><span data-stu-id="60ef0-136">displayName</span></span>|<span data-ttu-id="60ef0-137">String</span><span class="sxs-lookup"><span data-stu-id="60ef0-137">String</span></span>|<span data-ttu-id="60ef0-138">EBook カテゴリの名前です。</span><span class="sxs-lookup"><span data-stu-id="60ef0-138">The name of the eBook category.</span></span>|
|<span data-ttu-id="60ef0-139">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="60ef0-139">lastModifiedDateTime</span></span>|<span data-ttu-id="60ef0-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="60ef0-140">DateTimeOffset</span></span>|<span data-ttu-id="60ef0-141">日付と時刻、ManagedEBookCategory が最後に修正されました。</span><span class="sxs-lookup"><span data-stu-id="60ef0-141">The date and time the ManagedEBookCategory was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="60ef0-142">応答</span><span class="sxs-lookup"><span data-stu-id="60ef0-142">Response</span></span>
<span data-ttu-id="60ef0-143">かどうかは成功すると、このメソッドが返されます、`201 Created`応答コードおよび応答の本文に[managedEBookCategory](../resources/intune-books-managedebookcategory.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="60ef0-143">If successful, this method returns a `201 Created` response code and a [managedEBookCategory](../resources/intune-books-managedebookcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="60ef0-144">例</span><span class="sxs-lookup"><span data-stu-id="60ef0-144">Example</span></span>
### <a name="request"></a><span data-ttu-id="60ef0-145">要求</span><span class="sxs-lookup"><span data-stu-id="60ef0-145">Request</span></span>
<span data-ttu-id="60ef0-146">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="60ef0-146">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/managedEBookCategories
Content-type: application/json
Content-length: 166

{
  "@odata.type": "#microsoft.graph.managedEBookCategory",
  "displayName": "Display Name value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
}
```

### <a name="response"></a><span data-ttu-id="60ef0-147">応答</span><span class="sxs-lookup"><span data-stu-id="60ef0-147">Response</span></span>
<span data-ttu-id="60ef0-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="60ef0-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 215

{
  "@odata.type": "#microsoft.graph.managedEBookCategory",
  "id": "3c71fb14-fb14-3c71-14fb-713c14fb713c",
  "displayName": "Display Name value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
}
```





