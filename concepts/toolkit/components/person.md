---
title: Microsoft Graph ツールキットの Person コンポーネント
description: Person コンポーネントは、ユーザーまたは連絡先を、自分の写真、名前、電子メールアドレスを使用して表示するために使用されます。
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: b9102259258bb691dee2c56449257740db7b1913
ms.sourcegitcommit: 750c82f161a0f62bc2486995456ccd92ee5c7831
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/26/2019
ms.locfileid: "35243038"
---
# <a name="person-component-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="01737-103">Microsoft Graph ツールキットの Person コンポーネント</span><span class="sxs-lookup"><span data-stu-id="01737-103">Person component in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="01737-104">Person コンポーネントは、ユーザーまたは連絡先を、自分の写真、名前、電子メールアドレスを使用して表示するために使用されます。</span><span class="sxs-lookup"><span data-stu-id="01737-104">The person component is used to display a person or contact by using their photo, name, and/or email address.</span></span> 

## <a name="example"></a><span data-ttu-id="01737-105">例</span><span class="sxs-lookup"><span data-stu-id="01737-105">Example</span></span>

[<span data-ttu-id="01737-106">jsfiddle の例</span><span class="sxs-lookup"><span data-stu-id="01737-106">jsfiddle example</span></span>](https://jsfiddle.net/metulev/0jkzfr42/)

### <a name="add-the-control-to-the-html-page"></a><span data-ttu-id="01737-107">HTML ページにコントロールを追加する</span><span class="sxs-lookup"><span data-stu-id="01737-107">Add the control to the HTML page</span></span>
```html
<mgt-person person-query=""></mgt-person>
```

## <a name="setting-the-person-details"></a><span data-ttu-id="01737-108">個人情報の設定</span><span class="sxs-lookup"><span data-stu-id="01737-108">Setting the person details</span></span>

<span data-ttu-id="01737-109">3つのプロパティを使用して、人物の詳細を設定できます。</span><span class="sxs-lookup"><span data-stu-id="01737-109">You can use three properties to set the person details.</span></span> <span data-ttu-id="01737-110">インスタンスごとに、次のいずれかのプロパティを使用します。</span><span class="sxs-lookup"><span data-stu-id="01737-110">Use only one of the following properties per instance:</span></span>

* <span data-ttu-id="01737-111">`user-id`属性または`userId`プロパティを設定して、ID を使用して Microsoft Graph からユーザーを取得します。</span><span class="sxs-lookup"><span data-stu-id="01737-111">Set the `user-id` attribute or `userId` property to fetch the user from Microsoft Graph by using their ID.</span></span>  

* <span data-ttu-id="01737-112">特定の`person-query`ユーザーの`personQuery` Microsoft Graph を検索するように、属性またはプロパティを設定します。</span><span class="sxs-lookup"><span data-stu-id="01737-112">Set the `person-query` attribute or `personQuery` property to search Microsoft Graph for a given person.</span></span> <span data-ttu-id="01737-113">最初に使用可能な人物を選択し、ユーザーの詳細を取得します。</span><span class="sxs-lookup"><span data-stu-id="01737-113">It will choose the first person available and fetch the person details.</span></span> <span data-ttu-id="01737-114">電子メールは、適切な人物に対してクエリを実行することをお勧めしますが、名前も同じように動作します。</span><span class="sxs-lookup"><span data-stu-id="01737-114">An email works best to ensure the right person is queried, but a name works as well.</span></span>

* <span data-ttu-id="01737-115">次の`person-details`例に`personDetails`示すように、手動で個人情報を設定するように属性またはプロパティを設定します。</span><span class="sxs-lookup"><span data-stu-id="01737-115">Set the `person-details` attribute or `personDetails` property to manually set the person details, as shown in the following example.</span></span>


    ```js
    let personControl = document.getElementById('myPersonControl');
    personControl.personDetails = {
        displayName: 'Nikola Metulev',
        email: 'nikola@contoso.com',
        image: 'url'
    }
    ```

  <span data-ttu-id="01737-116">イメージが指定されていない場合は、取得されます (使用可能な場合)。</span><span class="sxs-lookup"><span data-stu-id="01737-116">If no image is provided, one will be fetched (if available).</span></span>

## <a name="changing-how-the-component-looks"></a><span data-ttu-id="01737-117">コンポーネントの外観の変更</span><span class="sxs-lookup"><span data-stu-id="01737-117">Changing how the component looks</span></span>

<span data-ttu-id="01737-118">複数のプロパティを使用して、コンポーネントをカスタマイズできます。</span><span class="sxs-lookup"><span data-stu-id="01737-118">You can use several propertiesto customize the component.</span></span>

| <span data-ttu-id="01737-119">プロパティ</span><span class="sxs-lookup"><span data-stu-id="01737-119">Property</span></span> | <span data-ttu-id="01737-120">属性</span><span class="sxs-lookup"><span data-stu-id="01737-120">Attribute</span></span> | <span data-ttu-id="01737-121">説明</span><span class="sxs-lookup"><span data-stu-id="01737-121">Description</span></span> |
| --- | --- | --- |
| `showName` | `show-name` | <span data-ttu-id="01737-122">ユーザーの表示名を表示するフラグを設定`false`します。既定値はです。</span><span class="sxs-lookup"><span data-stu-id="01737-122">Set flag to display person display name - default is `false`.</span></span> |
| `showEmail` | `show-email` | <span data-ttu-id="01737-123">ユーザーの電子メールを表示するフラグを`false`設定します。既定値はです。</span><span class="sxs-lookup"><span data-stu-id="01737-123">Set flag to display person email - default is `false`.</span></span> |

## <a name="css-custom-properties"></a><span data-ttu-id="01737-124">CSS カスタムプロパティ</span><span class="sxs-lookup"><span data-stu-id="01737-124">CSS custom properties</span></span>

<span data-ttu-id="01737-125">コンポーネント`mgt-person`は、次の CSS カスタムプロパティを定義します。</span><span class="sxs-lookup"><span data-stu-id="01737-125">The `mgt-person` component defines the following CSS custom properties.</span></span>

```css
mgt-person {
  --avatar-size-s: 24px;
  --avatar-size: 48px; // avatar size when both name and email are shown
  --avatar-font-size--s: 16px;
  --avatar-font-size: 32px; // font-size when both name and email are shown
  --avatar-border: 0;
  --initials-color: white;
  --initials-background-color: magenta;
  --font-size: 12px;
  --font-weight: 500;
  --color: black;
  --email-font-size: 12px;
  --email-color: black;
}
```

<span data-ttu-id="01737-126">詳細については、「[スタイルコンポーネント](../style.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="01737-126">To learn more, see [styling components](../style.md).</span></span>

## <a name="templates"></a><span data-ttu-id="01737-127">テンプレート</span><span class="sxs-lookup"><span data-stu-id="01737-127">Templates</span></span>

<span data-ttu-id="01737-128">コンポーネント`mgt-person`は、コンポーネントの特定の部分を置き換えることができるいくつかの[テンプレート](../templates.md)をサポートしています。</span><span class="sxs-lookup"><span data-stu-id="01737-128">The `mgt-person` component supports several [templates](../templates.md) that allow you to replace certain parts of the component.</span></span> <span data-ttu-id="01737-129">テンプレートを指定するには、 `<template>`コンポーネント内に要素を含め、 `data-type`値を次のいずれかに設定します。</span><span class="sxs-lookup"><span data-stu-id="01737-129">To specify a template, include a `<template>` element inside a component and set the `data-type` value to one of the following:</span></span>

| <span data-ttu-id="01737-130">データ型</span><span class="sxs-lookup"><span data-stu-id="01737-130">Data type</span></span> | <span data-ttu-id="01737-131">データコンテキスト</span><span class="sxs-lookup"><span data-stu-id="01737-131">Data context</span></span> | <span data-ttu-id="01737-132">説明</span><span class="sxs-lookup"><span data-stu-id="01737-132">Description</span></span> |
| --- | --- | --- |
| `default` | <span data-ttu-id="01737-133">`person`: person オブジェクト</span><span class="sxs-lookup"><span data-stu-id="01737-133">`person`: a person object</span></span> | <span data-ttu-id="01737-134">既定のテンプレートでは、コンポーネント全体が独自のものに置き換えられます。</span><span class="sxs-lookup"><span data-stu-id="01737-134">The default template replaces the entire component with your own.</span></span> |

<span data-ttu-id="01737-135">次の例では、person コンポーネントのテンプレートを定義します。</span><span class="sxs-lookup"><span data-stu-id="01737-135">The following example defines a template for the person component:</span></span>

```html
<mgt-person>
  <template>
    <div data-if="person.image">
      <img src="{{person.image}}" />
    </div>
    <div data-else>
      {{person.displayName}}
    </div>
  </template>
</mgt-person>
```

## <a name="microsoft-graph-permissions"></a><span data-ttu-id="01737-136">Microsoft Graph のアクセス許可</span><span class="sxs-lookup"><span data-stu-id="01737-136">Microsoft Graph permissions</span></span>

<span data-ttu-id="01737-137">このコントロールでは、次の Microsoft Graph Api とアクセス許可を使用します。</span><span class="sxs-lookup"><span data-stu-id="01737-137">This control uses the following Microsoft Graph APIs and permissions.</span></span>

| <span data-ttu-id="01737-138">リソース</span><span class="sxs-lookup"><span data-stu-id="01737-138">Resource</span></span> | <span data-ttu-id="01737-139">アクセス許可/スコープ</span><span class="sxs-lookup"><span data-stu-id="01737-139">Permission/scope</span></span> |
| - | - |
| [<span data-ttu-id="01737-140">/me</span><span class="sxs-lookup"><span data-stu-id="01737-140">/me</span></span>](https://docs.microsoft.com/en-us/graph/api/user-get?view=graph-rest-1.0) | `User.Read` |
| [<span data-ttu-id="01737-141">/me¥ photo/$value</span><span class="sxs-lookup"><span data-stu-id="01737-141">/me/photo/$value</span></span>](https://docs.microsoft.com/en-us/graph/api/profilephoto-get?view=graph-rest-beta) | `User.Read` |
| [<span data-ttu-id="01737-142">/me/people/? $search =</span><span class="sxs-lookup"><span data-stu-id="01737-142">/me/people/?$search=</span></span>](https://docs.microsoft.com/en-us/graph/api/user-list-people?view=graph-rest-1.0) | `People.Read` |
| [<span data-ttu-id="01737-143">/me/contacts/\*</span><span class="sxs-lookup"><span data-stu-id="01737-143">/me/contacts/\*</span></span>](https://docs.microsoft.com/en-us/graph/api/user-list-contacts?view=graph-rest-1.0&tabs=cs) | `Contacts.Read` |
| [<span data-ttu-id="01737-144">/ユーザー/_/_/_/$value</span><span class="sxs-lookup"><span data-stu-id="01737-144">/users/{id}/photo/$value</span></span>](https://docs.microsoft.com/en-us/graph/api/user-list-people?view=graph-rest-1.0) | `User.ReadBasic.All` |

> <span data-ttu-id="01737-145">**注:** 個人用の`*/photo/$value` microsoft アカウントのリソースにアクセスするには、microsoft Graph ベータ版エンドポイントを使用します。</span><span class="sxs-lookup"><span data-stu-id="01737-145">**Note:** to access the `*/photo/$value` resources for personal Microsoft accounts, use the Microsoft Graph beta endpoint.</span></span>

## <a name="authentication"></a><span data-ttu-id="01737-146">認証</span><span class="sxs-lookup"><span data-stu-id="01737-146">Authentication</span></span>

<span data-ttu-id="01737-147">このコントロールは、[認証のドキュメント](./../providers.md)で説明されているグローバル認証プロバイダを使用して、必要なデータをフェッチします。</span><span class="sxs-lookup"><span data-stu-id="01737-147">The control uses the global authentication provider described in the [authentication documentation](./../providers.md) to fetch the required data.</span></span>
